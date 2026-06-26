---
title: "Introducing OpenCR-MuJoCo"
toc: true
excerpt: "An open-source MuJoCo workflow for tendon-driven continuum robots, contact-rich manipulation, and reproducible benchmarking."
category: research
author: "cjs"
header:
  teaser: /assets/images/posts/research/mujoco/teaser.png
---

{% include figure popup=true image_path="/assets/images/posts/research/mujoco/teaser.png" %}


We are excited to introduce **OpenCR-MuJoCo**, an open-source project that brings tendon-driven continuum robots (TDCRs) into native MuJoCo through a mechanics-informed representation.

The motivation is simple. Continuum robots are compelling because they bend, conform, and make compliant contact along their whole body. That distributed compliance is one of the reasons they are promising for constrained manipulation, medical robotics, inspection, and delicate physical interaction.

It is also one of the reasons they are hard to simulate. For many existing learning and manipulation workflows, mature simulation infrastructure has become part of the research loop: fast rollouts, contact-rich scenes, robot arms, objects, actuators, teleoperation, and standard interfaces to learning code. In continuum robotics, we have a strong modeling foundation, but it is often harder to plug that foundation directly into the everyday simulation workflows used for contact-rich robot learning.

OpenCR-MuJoCo is our attempt to make that easier.

## Building on the Existing Foundation

Continuum robotics has benefited enormously from physically grounded simulation methods. Cosserat rod models, finite-element methods, discrete elastic rod formulations, and tools such as SoRoSim, SOFA, Elastica, DisMech, and related simulators have shaped how the field understands continuum robot mechanics. These methods remain important, and our work is very much built on the foundation they provide. Here, we ask a more infrastructure-oriented question:

**Can we put a TDCR directly inside MuJoCo in a way that is simple, fast, interpretable, and accurate enough to support real robot workflows?**

The answer we explore in OpenCR-MuJoCo is deliberately simple in nature. We discretize the continuum backbone into a serial chain of rigid links connected by elastic joints. The key is that the joint stiffnesses are derived from the robot's material and geometric properties, rather than treated only as arbitrary fit parameters. Tendons are routed through sites along the backbone and actuated using MuJoCo's native tendon model.

This lets the TDCR live as a native MuJoCo model: it can contact objects, share a scene with a robot arm, use standard MuJoCo actuators and tendons, and connect naturally to teleoperation and learning code. At the same time, the model keeps an interpretable relationship to the underlying continuum mechanics.

{% include figure popup=true image_path="/assets/images/posts/research/mujoco/method.png" caption="Mechanics-informed TDCR discretization and native MuJoCo integration."%}

## What We Contribute

The main contribution is a practical way to represent and use TDCRs inside native MuJoCo, built around this mechanics-informed discretization.

On the modeling side, the TDCR backbone is represented by rigid links and elastic joints whose stiffness comes from beam theory. As the discretization is refined, the approximation converges toward the continuum rod model, while each parameter still has a physical interpretation. In practice, this gives a useful balance: the model is simple enough to run quickly inside MuJoCo, but structured enough that changing material, geometry, tendon routing, or discretization resolution remains meaningful.

On the systems side, the model is encoded in standard MJCF and uses MuJoCo's existing physics pipeline. That means native tendon actuation, contact handling, rigid-object interaction, and robot-arm integration happen in one MuJoCo scene. For contact-rich manipulation, this is especially useful: the contact locations and forces do not need to be specified ahead of time, but can emerge from the interaction between the compliant robot body, the objects, and the environment.

This is the part we are most excited about for the community. If continuum robots can be easier to instantiate, control, validate, and benchmark in a common simulation environment, then more researchers can compare methods on shared tasks instead of rebuilding similar infrastructure from scratch.

## Validation: From Mechanics to Hardware to Policies

A modeling workflow only becomes useful when researchers can trust it for the questions they want to ask. For OpenCR-MuJoCo, we evaluated that trust at three levels.

First, we compare against **SoRoSim**, a well-established Cosserat rod simulator. This is an important reference point because it tests whether the MuJoCo discretization behaves like a continuum-mechanics model, not merely whether it looks plausible. We evaluate static equilibrium shapes and dynamic tip-release trajectories across two materials spanning a large stiffness range, randomized loading conditions, and multiple discretization resolutions. In the practical operating regime used in our experiments, the static and dynamic errors are below 1% of robot length while maintaining real-time simulation.

<table>
  <tr>
    <td width="50%">
      <img src="/assets/images/posts/research/mujoco/sorosim_statics_shapes.png" alt="Static TDCR shapes from MuJoCo compared with SoRoSim references." />
    </td>
    <td width="50%">
      <img src="/assets/images/posts/research/mujoco/sorosim_statics_error.png" alt="Static tip error versus discretization resolution." />
    </td>
  </tr>
</table>


{% include figure popup=true image_path="/assets/images/posts/research/mujoco/sorosim_dynamics_overview.png" caption="Dynamic tip-release trajectories from MuJoCo compared with SoRoSim references."%}


Second, we compare against **real hardware**. We calibrate the MuJoCo model to a physical three-segment, nine-tendon TDCR. After system identification, the model reaches a mean tip tracking error of about 7.7 mm, or 4.1% of the 186.5 mm robot length, on held-out hardware data. This test is important because real TDCRs include effects that are difficult to model perfectly, such as friction, hysteresis, assembly tolerances, and tendon pretension.

Third, we test whether the native MuJoCo representation is useful for **policy learning and sim-to-real transfer**. We collect teleoperated demonstrations in simulation, train state-based imitation-learning policies, and deploy them zero-shot on the physical robot. The tasks are intentionally contact-rich: one policy wraps the continuum body around a cylinder to lift and drop it into a bin, while another flips a small wall-mounted switch from behind. In the reported experiments, real-world success rates match or slightly exceed simulation: 76% for the grasping task and 78% for the switch task.

<video src="/assets/images/posts/research/mujoco/opencr_mujoco_video.mp4" controls muted playsinline poster="/assets/images/posts/research/mujoco/opencr_mujoco_video_poster.jpg" style="display:block; width:100%; height:auto;"></video>


We see this policy transfer as the ultimate practical test of the approach. Matching a reference model is necessary, and matching hardware trajectories is encouraging, but contact-rich manipulation asks whether the MuJoCo integration supports a full research workflow: model generation, calibration, teleoperation, data collection, policy training, and real robot deployment.

## What Is Included

OpenCR-MuJoCo is meant to be research infrastructure, not just a static release for one paper. The repository includes:

- A config-driven TDCR generator for material-based stiffness, pretension, collision settings, and modular heterogeneous robots.
- Native MuJoCo scenes for TDCR-only setups and TDCRs mounted on a Franka Panda arm.
- Teleoperation and controller tools for joint- and task-space TDCR control.
- Evaluation scripts and bundled reference data for reproducing the validation.

For a new user, the intended workflow is lightweight: choose a JSON configuration, generate a MuJoCo scene, and run it with our teleop controller or a custom control loop.

<table>
  <tr>
    <td width="33%">
      <img src="/assets/images/posts/research/mujoco/tdcr_tip_trace.gif" alt="Closed-loop TDCR tip tracing." />
    </td>
    <td width="33%">
      <img src="/assets/images/posts/research/mujoco/franka_tdcr_trace.gif" alt="Station keeping while the Franka arm moves." />
    </td>
    <td width="33%">
      <img src="/assets/images/posts/research/mujoco/kick_goal.gif" alt="Elastic kick interaction demo." />
    </td>
  </tr>
</table>

## Our Vision for Future Work

We are releasing OpenCR-MuJoCo because we want continuum robotics to have simulation infrastructure that is easier to use, easier to reproduce, and easier to benchmark with.

Many groups build different TDCRs with different tendon routings, different materials, and for different tasks. That diversity is valuable. At the same time, it can make methods difficult to compare. We hope OpenCR-MuJoCo can provide one useful common ground.

There is still a lot to do. OpenCR-MuJoCo currently focuses on slender tendon-driven continuum robots where the Kirchhoff rod assumptions are appropriate. Other soft robot morphologies, richer sensing, shape feedback, vision-based policies, broader benchmarks, and deeper comparisons between learning methods are all open directions.

If you work on continuum robot modeling, control, learning, hardware design, or benchmarking, we would love for you to try it and tell us what would make it more useful. Bug reports, feature requests, benchmark ideas, new robot configurations, and pull requests are all welcome.

Try the demo, clone the repository, reproduce the validation, or build a model of your own TDCR! We are looking forward to seeing what the community does with it.

[Project Page](https://continuumroboticslab.github.io/opencr-mujoco/){: .btn .btn--success}
[GitHub](https://github.com/ContinuumRoboticsLab/opencr-mujoco){: .btn .btn--danger} 
[Paper](https://arxiv.org/abs/2606.22397){: .btn .btn--info} 
