---
title: "Beyond Medical Applications"
author: jbk
toc: false
classes: wide
category: opinion
excerpt: Opportunities for continuum robotics are largely unexploited, as the medical focus restricts and constrains innovation.
header:
  teaser: /assets/images/posts/opinion/hologram-interface-in-office-overlooking-city-4562612_teaser.jpg
---
Research on continuum robots has been primarily focussed on medical robotics. The common use case involes a physician teleoperating the continuum robot, who is in full control at all times. For instance in interventional medicine, a robotically-steered catheter or bronchoscope is essentially a long continuum robot whose tip is articulated while navigating through the vasculature or the airways. Although use in medical robotics is compelling, I argue that the opportunity space for continuum robotics remains largely unexploited as the medical focus restricted and constrained innovation in robot embodiment, control strategies, level of autonomy, and available feedback. 

## Why are Continuum Robots predominantly explored for medicial applications?
Looking at the history of continuum robotics, early research has focussed on larger scale continuum robots. Prototypes were built comparable in size to industrial serial arm robots. This probably resulted in expectations in terms of performance. If an industrial robot arm could achieve superior accuracy and repeatabilty with high payloads and at high speed, why would one need a continuum robot performing worse on this scale? Repeatability, accuracy, speed, and payload are clearly not unique selling points for continuum robots. Poised by the third industrial revolution in the late sixties and early seventies of the 20th century, roboticists naturally focussed on robots applicable to automation and its goals. Continuum robots were just not cutting it (yet). Consequently, continuum robotics remained a niche research area for a while.

Medical robotics was just on the onset in the mid eighties and was using repurposed industrial robots. The first medical robotics procedure used the PUMA 560 robot to perform a neurosurgical biopsy at the National Hospital for Neurology and Neurosurgery in London in 1985. The robot guided a needle into the brain to take a tissue sample for examination. Fun fact: The Puma 560 design is based on an earlier robot design by Victor Scheinman, the same Victor Scheinman who developed the [first continuum robot](https://www.cs.toronto.edu/~jbk/opencontinuumrobotics/history/2022/11/01/ORM.html).

The trend towards more minimally invasive surgey and ultimatley keyhole access to operate promises benefits for patient care, such as shorter hopsitalization and quicker recovery times. While industrial style robots certainly play an important role in medical robotics today, their large footprint and size naturally places them beside physicians and outside of the patient. But as soon as one wants to move away from large incisions and the need to open the body, thin, versatile, and dextrous robotics enters the scene. Small-scale continuum robots could sneak into a patient with more dextrous motion capabilties than conventional robots and the ability to reach surgical sites inaccessible by conventional robots or standard medical instruments! And that ability is more defining than accuracy and payload. In contrast to industrial automation, small-scale continuum robots promise significant benefit over serial robot arms! 

With medical applications, continuum robots found a compelling use case. Motivated by unsought of minimally-invasie approaches and the ability to navigate within the human body through natural orifices or miniscule inscisions, research in continuum robotics excelled. Over the past decades we have witnessed a vast surge in medical continuum robots. In fact, the majority of continuum robot papers draw their motivation from medical applications. The prominent surveys in the field of continuum robotics are centered around medicine[^BurgnerKahrs2015] [^daVeiga2020] [^Dupont2022] and I refer the interested reader to those surveys to learn about the breadth and depth of medical continuum robotics research. 

## The Untapped Potential
One may argue that continuum robots found their sweet spot in the medical application domain. While this is certainly the case, the untapped potential of continuum robots in non-medical applications is enormous! Think about autonomous small-scale or medium-scale continuum robots in in-situ and non-destructive inspection, maintenance, repair, and operations. 

**Example**: On-wing jet engine inspection provides an example of a keyhole procedure, where a technician inspects components such as  turbine blades and the combustion chamber using a flexible camera, called a borescope, through tiny access points on the engine. This is a cumbersome procedure requiring an expert to fiddle with the borescope in hunched body postures, with limited time, as the plane stands ready for takeoff. If an issue is overlooked, e.g., a small crack in a blade, it may be disastrous and result in a worst-case scenario of the engine blowing off during flight. At the same time, full service of an engine means that it must be taken off-wing for maintenance – a costly endeavour. Only very few researcher worldwide look at this problem, with the University of Notthingham spearheading research with Rolls Royce on [robotics for in-situ repair](https://www.nottingham.ac.uk/utc/research/robotics-for-in-situ-repair/robotics-for-in-situ-repair.aspx)
{: .notice}

This in-situ inspection is just one of many examples where we can build on our expertise in continuum robotics in the medical domain and innovate the next generation of autonomous continuum robot systems. 
In fact, non-medical applications for continuum robots are characterized by similar challenges: 

- limited accessiblity,
- tortuous pathways in constrained environments, and
- need for dextrous manipulation at the location of interest.

At the same time, turning to new application domains opens new research questions challenging to solve:

- How can we design long continuum robots that can maintain stability?
- How can we avoid buckling for continuum robots navigating cluttered environments?
- How can we achieve dextrous steering and motion capalities and bear sufficient loads?

I envision a new generation of continuum robots that are of small and medium scale, dextrous enough to enter an environment for in-situ inspection, maintenance, and repair through multiple keyholes, which act autonomously and are able to collaborate with one another to achieve the task. 


## Call to Action
I believe, that we as the continuum robotics community, should turn to non-medical use-cases to invent this next-generation of continuum robot systems with autonomous capabilities. By focussing on medical applications, we have naturally limited our design choices to certain continuum robot dimensions, materials, workspaces, control paradigms, etc. that are informed by anatomical constraints and clinical requirements. In fact, most medical continuum robots are rather short if they can are designed to work in free spaces. Longer medical continuum robots need environmental constraints for steering - such as vasculature for robotic catheters. 

Drawing motivation from one application domain lead to narrow thinking and limited creativity. Continuum robotics researchers and innovators have become too focused on the specific needs and constraints of medicine. I argue that this prevented us from considering new and unconventional ideas!

Overall, while focusing on medicine as the dominant application domain was necessary to develop expertise in continuum robotics, it is important for the continuum robotics community to maintain a broad perspective and engage with other fields and industries to encourage innovation and avoid limiting the potential for new and unconventional ideas.

## References
[^BurgnerKahrs2015]: J. Burgner-Kahrs, D.C. Rucker, and H. Choset: Continuum Robots for Medical Applications: A Survey. IEEE Transactions on Robotics, 31(6), pp.1261–1280. doi: [10.1109/TRO.2015.2489500](https://doi.org/10.1109/TRO.2015.2489500) 

[^daVeiga2020]: T. da Veiga, J.H. Chandler, P. Lloyd, G. Pittiglio,  N.J. Wilkinson, A.K. Hoshiar, R.A. Harris, and P. Valdastri: Challenges of continuum robots in clinical context: a review. Progress in Biomedical Engineering, 2(3): 032003, 2020. doi: [10.1088/2516-1091/ab9f41](https://doi.org/10.1088/2516-1091/ab9f41)

[^Dupont2022]: P.E. Dupont, N. Simaan, H. Choset, and D.C. Rucker: Continuum robots for medical interventions. Proceedings of the IEEE, 110(7):847-870, 2022. [10.1109/JPROC.2022.3141338](https://doi.org/10.1109/JPROC.2022.3141338)