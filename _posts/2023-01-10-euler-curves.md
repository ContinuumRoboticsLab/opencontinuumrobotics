---
title: "Representing the Backbone of Tendon-driven Continuum Robots using Euler Curves"
author: pr
toc: true
category: research
excerpt: Euler curves are a more powerful representation than constant curvature arcs to represent the shape of a continuum robot.
header:
    teaser: /assets/images/posts/research/euler-curve-hook.png
---
In one of the earlier posts, we learnt about the [constant curvature
(CC) representation]({% post_url /2022-12-02-cc-kinematics %}).
The approach assumes that the entire backbone can be represented as a
circular arc, requiring two parameters in 3D space. From the
Euler-Bernoulli theorem we know that the curvature of the beam is
directly proportional to the moment experienced by it. Therefore, the CC
representation can only model a constant planar moment experienced by
the robot.

Due to its simplistic formulation, the CC is one of the most common
backbone approximations made in literature. It has been shown that if
there is no external gravitational, frictional, applied forces on the
backbone, the tendon forces can be approximated by a constant moment
applied on the segment [^Camarillo2008]. Since it requires only two
parameters to represent the robot and uses geometrical assumptions, many
closed form analytical models have been proposed that are
computationally inexpensive as the formulation can be expressed as
matrix operations. 

However, if the robot is carrying a tool or camera at
its tip for inspection and other tasks, there is bound to be a variation
in curvature as shown below, and results in deviation from the CC shape.

|![img]({{ site.url }}{{ site.baseurl }}/assets/images/posts/research/euler-curve-hook.png)|
|Shape of a TDCR under different tip forces. The backbone can be approximated by the Euler Arc Spline representation as a series of $$n$$ arcs with curvatures in arithmetic progression. When no force is applied, the robot curvature is constant (green) and $$\kappa_1=\kappa_n$$. As the force increases, so does the variation in curvature (red)|


At ICRA 2019, Euler curves were proposed to represent long, heavy
continuum robots [^Gonthina2019]. These are curves that have a linearly
varying curvatures. Since long heavy continuum robots bend under the
influence of gravity, we hypothesized [^Rao2021a] [^Rao2022] that they
can be used to represent the backbone experiencing an external force at
the tip as well.

## Euler Arc Spline representation

When using Euler curves, the robot-independent mapping (configuration to task space)
requires Fresnel integration which can add to the
computation. In order to retain the advantage of the CC representation,
where the configuration to task space mapping is computed by efficient
matrix operations, we use the Euler Arc Spline (EAS) representation.
This EAS representation of an Euler curve was first proposed by Meek and Walton
[^Meek2004] in the context of clothoids. To represent a continummum robot backbone with EAS, we use a series of arcs whose
curvatures are linearly constrained and assumed to be in arithmetic progression as illustrated here:

|![img]({{ site.url }}{{ site.baseurl }}/assets/images/posts/research/euler_curve_fig1.png)|![img]({{ site.url }}{{ site.baseurl }}/assets/images/posts/research/euler_curve_fig2.png)|
|CC representation|EAS representation|

The proposed representation can be extended to 3D by linearizing the
components of curvature along all three axes, resulting in 6 parameters
in total (two along each axes). 

The EAS representation was tested on a set of 70 spatial TDCR deformations with two identical TDCR prototypes, operating both in free space and under the influence of an external tip force. It was found to represent the backbone shape with an average tip error of less than 0.5%. This result indicates that EAS is a powerful representation for continuum robots experiencing tip forces that cannot be achieved with CC represenations.

|![img]({{ site.url }}{{ site.baseurl }}/assets/images/posts/research/euler_curve_comp_time.png)|
|Computation times of three models - EAS (red), CRT (black), and PCCA (blue) with increasing number of disks for planar (left) and non-planar (right) deformations.|

## Potential

One of the major advantages of the backbone representation simplification is the
reduced parameterization, without significant trade-off in accuracy. The
lower number of unknowns offers the advantage of reduced computational
time for a physics based model. Another advantage lies in its use in
data-driven models. Lower number of configuration parameters requires
lesser number of data points to train different models, allowing us to
learn the behaviour of these robots due to unmodelled factors like
manufacturing and assembly errors.

While we show the potential of Euler curves for TDCR experiencing tip forces, there are
multiple avenues where its advantages could be exploited. It could be
extended to model multiple forces along the backbone. Applying them for
helical routing and learning their behaviour could be investigated to
find the optimum routing to reach a particular target.

![img]({{ site.url }}{{ site.baseurl }}/assets/images/posts/research/euler_curve_table.png){: .align-center}

***Further Reading:*** Curious to learn more about the use of Euler Arc Splines to model tendon-driven continuum robots? We published our finding in the IEEE Robotics & Automation Letters[^Rao2022] and presented our work at the IEEE International Conference on Intelligent Robots and Systems in 2022. For a quick summary, watch the video recording below! 
[Paper](https://www.cs.toronto.edu/~jbk/pubs/2022_Rao_TDCR-EAS_RAL_preprint.pdf){: .btn .btn--info} 
[Video](https://youtu.be/kavIG50nVb0){: .btn .btn--success}
{: .notice--success}

{% include video id="kavIG50nVb0" provider="youtube" %}

## References
[^Camarillo2008]: D. B. Camarillo, C. F. Milne, C. R. Carlson, M. R. Zinn, J. K. Salisbury: Mechanics modeling of tendon-driven continuum manipulators. IEEE Transactions on Robotics, 24(6):1262–1273, 2008. doi: [10.1109/TRO.2008.2002311](https://doi.org/10.1109/TRO.2008.2002311)

[^Gonthina2019]: P. S. Gonthina, A. D. Kapadia, I. S. Godage, I. D. Walker: Modeling variable curvature parallel continuum robots using euler curves. IEEE International Conference on Robotics and Automation, pp. 1679–1685, 2019. doi: [10.1109/ICRA.2019.8794238](https://doi.org/10.1109/ICRA.2019.8794238)

[^Rao2021a]: P. Rao, Q. Peyron, S. Lilge, J. Burgner-Kahrs: How to Model TendonDriven Continuum Robots and Benchmark Modelling Performance. Frontiers in Robotics and AI, vol. 7, p. 223, 2021. doi: [10.3389/frobt.2020.630245](https://doi.org/10.3389/frobt.2020.630245)

[^Rao2022]: P. Rao, Q. Peyron, and J. Burgner-Kahrs: Shape representation and modeling of tendon-driven continuum robots using euler arc splines. IEEE Robotics and Automation Letters, 7(3):8114–8121, 2022. doi: [10.1109/LRA.2022.3185377](https://doi.org/10.1109/LRA.2022.3185377)

[^Meek2004]: D. S. Meek and D. J. Walton: An arc spline approximation to a clothoid. Journal of Computational and Applied Mathematics, 170(1):5977, 2004. doi: [10.1016/j.cam.2003.12.038](https://doi.org/10.1016/j.cam.2003.12.038)