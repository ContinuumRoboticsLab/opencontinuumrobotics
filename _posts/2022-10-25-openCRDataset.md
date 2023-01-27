---
title: "Open-source Modeling Dataset"
author: jbk
toc: false
classes: wide
category: research
excerpt: The first public dataset for a concentric tube continuum robot to democrotize research on their learning-based and physics-based modeling.
header:
  teaser: /assets/images/posts/research/dataset_teaser.jpg
---
Establishing a physics-based model capturing the kinetostatic behavior of concentric tube continuum robots is challenging as elastic interactions between the flexible tubes constituting the robot result in a highly non-linear problem. The Goldstandard physics-based model using the Cosserat theory of elastic rods achieves reasonable approximations with 1.5 − 3% with respect to the robot’s length, if the model parameters are well tuned and the system is well-calibrated. Learning-based models of concentric tube continuum robots have outperformed the Goldstandard model with approximation errors below 1%. Yet, the merits of learning-based models remain largely unexplored as no common dataset and benchmark exist. Until now: We are releasing world's first public dataset for concentric tube continuum robots!

[![GitHub]({{ site.url }}{{ site.baseurl }}/assets/images/posts/research/github_link_image.jpg)](https://github.com/ContinuumRoboticsLab/CRL-Dataset-CTCR-Pose)

The dataset was captured from a three-tube concentric tube continuum robot for use in learning-based kinetostatic modeling research. It consists of 100,000 joint configurations and the corresponding 6-dof pose measurements (base and end of each tube) measured with an electromagnetic tracking system. This was a great Continuum Robotics Laboratory team effort spearheaded by [Reinhard Grassmann](https://reinhardgrassmann.github.io) with Ryan Chen and Nan Liang funded by the Natural Sciences and Engineering Research Council of Canada (NSERC). We share our insights on suitable joint space and task space representations as well as one-shot sampling methods in the corresponding paper[^fn1] alongside benchmarking results.

[Paper](https://www.cs.toronto.edu/~jbk/pubs/2022_Grassmann_DatasetAndBenchmarkCTCR_IROS.pdf){: .btn .btn--info} 
[Video](https://youtu.be/vP3yqEIiH-Q){: .btn .btn--success}

{% include video id="vP3yqEIiH-Q" provider="youtube" %}

***Note:*** While the paper[^fn1] was in press for IROS, we presented it at a workshop @RSS 2022:
Reinhard M. Grassmann, Ryan Zeyuan Chen, Nan Liang, and Jessica Burgner-Kahrs: A Dataset and Benchmark for Learning the Kinematics of Concentric Tube Continuum Robots. Robotics: Science and Systems -- Workshop on Learning from Diverse, Offline Data (L-DOD), 2022. [pdf](https://openreview.net/pdf?id=DW9uz_GZ0og) ***Cite the IROS Paper!***
{: .notice}

## References
[^fn1]: Reinhard M. Grassmann, Ryan Zeyuan Chen, Nan Liang, and Jessica Burgner-Kahrs: A Dataset and Benchmark for Learning the Kinematics of Concentric Tube Continuum Robots. IEEE/RSJ International Conference on Intelligent Robots and Systems, 2022. doi: [tbd](https://dx.doi.org/tbd).