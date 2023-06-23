---
title: "One Actuation Module to Create them All"
author: rmg
toc: false
classes: wide
category: hands-on
excerpt: An open actuation module to create your continuum robots. One for all!
header:
  teaser: /assets/images/posts/hands-on/one-module-teaser.jpeg
---
We are excited to announce that our open continuum robotics hardware is now out. It has been a humbling long journey that lead to our manuscript (which is now in review but available as pre-print on arXiv[^arXiv2023]). To increase the reproducibility and accessibility of continuum robotics research, we release the hardware design, component lists, assembly instructions, and software open source here on our website.

![]({{ site.url }}{{ site.baseurl }}/assets/images/posts/hands-on/one-module-teaser.jpeg)

As you are reading this on our blog, you are already aware of our initiative called the OpenCR Project. With this week's post, we are releasing our open actuation module [^arXiv2023] for the continuum robotics community to build torque-controlled continuum robots. The actuation module is capable of measuring the external torque as demonstrated with very simplified toy examples. Its versatile and modular characteristics are highlighted by building three different types of continuum robot prototypes. The presented prototypes are capable of torque control and fast trajectory tracking making them the first of a kind of the respective continuum robot type.

## The Why
Stepping aside, what problem are we actually addressing? In short -- the lack of torque-controlled continuum robot prototypes available to all researchers. In fact, this lack is grounded on two observations we made by observing our research community and relating to other research areas in robotics.

First, in our previous study [^WS_RSS_2020], we observed that precious time and focus are devoted to building custom prototypes. One can acknowledge that experiments on physical hardware in robotics are necessary and valuable for evaluations. However, over 60% of all prototypes are used for only a single publication. This demonstrates an inefficient habit of not reusing existing prototypes. Thus, a significant amount of time is devoted to creating proprietary hardware and software. This large and growing number of ***single-use prototypes*** imposes a barrier for the research community shifting away time and efforts from important research questions.

![]({{ site.url }}{{ site.baseurl }}/assets/images/posts/hands-on/reused_robot_over_time.png)

Second, on a more personal note, having the opportunity [^RoboterFabrik], [^TeachingLab] to regularly work with torque-controlled manipulators such as the Franka Emika Panda[^16], utilizing torque control for continuum robots seems to be a natural next stepping stone. Torque control has a rich history, especially for serial kinematic mechanisms [^13] [^14] [^15] [^16]. However, for some reason, the spread and success of torque-control used in pHRI (physical human-robot interaction) research has not reached our continuum robotics community. Perhaps, one reason is that not much time has been directed to build a continuum robot prototype capable of torque control. 

## The OpenCR Actuation Module
To provide torque-controlled continuum robot prototypes, we propose a modular actuation module consisting of a high-torque brushless electric motor, a high-resolution optical encoder, and a low-gear-ratio transmission. This choice of hardware allows for torque control and fast trajectory tracking in real time. Furthermore, it enables proprioceptive torque sensing by measuring motor currents without relying on additional sensors, e.g., tension sensors or load cells. In addition, the actuation module and its coupling system can be used in different actuation modes for a wide range of continuum robots. For instance, tendon displacement/tension and backbone rotation/torque can be controlled and measured.

![]({{ site.url }}{{ site.baseurl }}/assets/images/posts/hands-on/one-module-assembly.gif)

Recapping the technological trend towards torque-controlled robot systems in other research fields, we are forecasting a likely impact of the proposed actuation module and continuum robot prototypes built on it. The manuscript [^arXiv2023] takes initial steps towards advanced control methodologies. We are confident that the ability of continuum robots utilizing our actuation module (or one with similar capabilities) has a decisive advantage over previous existing prototypes. For example, a CTCR can detect external disturbance as shown here:

![]({{ site.url }}{{ site.baseurl }}/assets/images/posts/hands-on/one-module-ctcr-snap.gif)

## One Actuation Module to Create them All
The actuation module is modular and as such allows you to build any (!?) continuum robot. In the nature of the OpenCR project, we build three different types of continuum robots -- a parallel CR, a spatial TDCR, and a CTCR. The image below shows renderings and respective prototypes. By providing open-source hardware and software, we hope that this minimizes the repetitive tasks of developing prototypes, allowing researchers worldwide to focus on the main research challenges in continuum robotics. As a welcome side effect, robot-based evaluations can be performed quickly and become reproducible by other groups!

![]({{ site.url }}{{ site.baseurl }}/assets/images/posts/hands-on/one-module-create-all.jpeg)

To improve our prototypes, we took great inspiration from the Open Dynamic Robot Initiative, where efforts are made to build cost-efficient actuators for torque-controlled legged robots [^12] and manipulators [^6]. As a matter of fact, open robot hardware projects proliferate progress in robotics [^RAM_Survey_2023]. Therefore, we encourage you -- dear reader -- to participate in the development of open-source software and hardware as well as to join the journey of leveraging torque-controlled prototypes. Let's pave the way with new stepping stones toward untapped or under-investigated research directions.

We hope that the open source nature will bear fruit by opening untapped or under-investigated research directions related to dynamics and advanced control of continuum robots. 

[Paper](https://arxiv.org/pdf/2304.11850.pdf){: .btn .btn--info} 
[GitHub](https://github.com/ContinuumRoboticsLab/OpenCR-Hardware){: .btn .btn--danger} 
[Video](https://youtu.be/0MefE64Gw0U){: .btn .btn--success}


## References
[^arXiv2023]: Reinhard M. Grassmann, Chengnan Shentu, Taqi Hamoda, Puspita Triana Dewi, Jessica Burgner-Kahrs. "Open Continuum Robotics -- One Actuation Module to Create them All," 2023, arXiv: [2304.11850](https://arxiv.org/abs/2304.11850)

[^RoboterFabrik]: Sami Haddadin, Lars Johannsmeier, Johannes Schmid, Tobias Ende, Sven Parusel, Simon Haddadin, Moritz Schappler, Torsten Lilge, and Marvin Becker. "roboterfabrik: A pilot to link and unify german robotics education to match industrial and societal demands." International Conference on Robotics and Education, 2018. DOI: [10.1007/978-3-319-97085-1_1](https://doi.org/10.1007/978-3-319-97085-1_1)

[^TeachingLab]: Kristy Strauss, "‘It’s a really cool place’: U of T Mississauga students get hands-on experience in new robotics teaching lab." Accessed: April 25, 2023 [Online](https://www.utoronto.ca/news/it-s-really-cool-place-u-t-mississauga-undergrads-get-hands-experience-new-robotics-teaching)

[^WS_RSS_2020]: R. M. Grassmann, S. Lilge, P. Le, and J. Burgner-Kahrs, "CTCR prototype development: An obstacle in the research community?” in Robotics Retrospectives Workshop at RSS, 2020. [Online](https://openreview.net/forum?id=bYLFxFQPFtX)

[^RAM_Survey_2023]: V. V. Patel, M. V. Liarokapis, and A. M. Dollar, “Open robot hardware: Progress, benefits, challenges, and best practices,” IEEE Robotics & Automation Magazine, pp. 2–9, 2022. DOI: [10.1109/MRA.2022.3225725](https://doi.org/10.1109/MRA.2022.3225725)

[^6]: M. Wüthrich, F. Widmaier, F. Grimminger, J. Akpo, S. Joshi, V. Agrawal, B. Hammoud, M. Khadiv, M. Bogdanovic, V. Berenz, J. Viereck, M. Naveau, L. Righetti, B. Schölkopf, and S. Bauer, “Trifinger: An open-source robot for learning dexterity,” in Conference on Robot Learning, 2020. arXiv: [2008.03596](https://doi.org/10.48550/arXiv.2008.03596)

[^12]: F. Grimminger, A. Meduri, M. Khadiv, J. Viereck, M. Wüthrich, M. Naveau, V. Berenz, S. Heim, F. Widmaier, T. Flayols, J. Fiene, A. Badri-Spröwitz, and L. Righetti, “An open torque-controlled modular robot architecture for legged locomotion research,” IEEE Robotics and Automation Letters, vol. 5, no. 2, pp. 3650–3657, 2020. DOI: [10.1109/LRA.2020.2976639](https://doi.org/10.1109/LRA.2020.2976639)

[^13]: J. Luh, W. Fisher, and R. Paul, “Joint torque control by a direct feedback for industrial robots,” Transactions on Automatic Control, vol. 28, no. 2, pp. 153–161, 1983. DOI: [10.1109/TAC.1983.1103215](https://doi.org/10.1109/TAC.1983.1103215)

[^14]: L. E. Pfeffer, O. Khatib, and J. Hake, “Joint torque sensory feedback in the control of a PUMA manipulator,” IEEE Transactions on Robotics and Automation, vol. 5, no. 4, pp. 418–425, 1989. DOI: [10.1109/70.88056](https://doi.org/10.1109/70.88056)

[^15]: R. Bischoff, J. Kurth, G. Schreiber, R. Koeppe, A. Albu-Schäffer, A. Beyer, O. Eiberger, S. Haddadin, A. Stemmer, G. Grunwald, and G. Hirzinger, “The kuka-dlr lightweight robot arm-a new reference platform for robotics research and manufacturing,” in International Symposium on Robotics, 2010, pp. 1–8. [online](https://ieeexplore.ieee.org/document/5756872)

[^16]: S. Haddadin, S. Parusel, L. Johannsmeier, S. Golz, S. Gabl, F. Walch, M. Sabaghian, C. Jaehne, L. Hausperger, and S. Haddadin, "The Franka Emika Robot: A reference platform for robotics research and education," IEEE Robotics & Automation Magazine, vol. 29, no. 2, pp. 46-64, 2022. DOI: [10.1109/MRA.2021.3138382](https://doi.org/10.1109/MRA.2021.3138382)
