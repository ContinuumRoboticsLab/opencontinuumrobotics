---
title: "Motion Primitives"
author: jbk
toc: true
category: 101
header:
  teaser: /assets/images/posts/cr_motion_primitives_teaser.png
---
*What are the motion capabilities of a continuum robot?*

The ultimate goal of continuum robotics is to have a continuously bending manipulator such that its shape is fully controllable. Ideally, such a robot would be appearing as a ﬂexible cylindrical structure of soft material with its current state dictated by infinitely many actuators. Three main challenges are associated with this idealized continuum robot:
1. From a mechanical standpoint, the design space to achieve continuously bending structures and compliance is very large.

2. Design of robots in absence of rigid elements is unfamiliar as the vast majority of existing robots is rigid, stiﬀ, and well deﬁned.

3. While a continuum structure may in principle have an inﬁnite number of degrees of freedom in that it can bend, twist, contract, and eventually shear at any point along it, we will only be able to control a ﬁnite number of degrees of freedom by actuators.


The defining feature of a continuum robot is a continuously curving core structure, often referred to as backbone, whose shape can be actuated in some way. An almost universal additional property is that the backbone is compliant; that is, it yields smoothly to externally applied loads. Such a continuous structure has an inﬁnite dimensional configuration or shape space - at least in principle. In fact, only a ﬁnite number of degrees of freedom (DOF) are controllable/actuatable due to mechanical constraints in building continuum robots. If a continuum robot is controlled discretely (restricting the allowable shapes of the robot to a finite set, or a shape set defined by a finite set of inputs) then it will not only be much easier to realize from a mechanical standpoint, but also be much easier to control. Nevertheless, the compliance inherent in the continuum structure still allows the robot to adapt to contact with its environment and to compensate for the limitations in its actuatable degrees of freedom.

The motion capabilities of a continuum robot can be expressed by a set of motion primitives:

**Extension and Contraction** to change the length along one axis.

**Bending** in one plane (i.e. rotation about one axis) or spatially (i.e. rotation about two axes).

**Twisting** about the longitudinal axis (i.e. turning or torsion)

|  ![image]({{ site.url }}{{ site.baseurl }}/assets/images/posts/cr_motion_primitives.png){: style="float: left"} |
| Motion primitives: change of length, bending in one planar or spatially, and torsion. |

These motion primitives can be combined and realized in a single continuum robot segment. The Figure below shows some examples. For instance, a continuum robot segment can bend in one plane and change its length or bend spatially and change its length. 

| ![image]({{ site.url }}{{ site.baseurl }}/assets/images/posts/cr_motion_primitives_combined.png){: style="float: left"} |
| Examples of motion capabilities for a single continuum robot segment. |

To increase the range of motion of a continuum robot, we can stack multiple of these segments, i.e. arrange them in series.

| ![image]({{ site.url }}{{ site.baseurl }}/assets/images/posts/cr_motion_primitives_stacked.png){: style="float: left"} |
| Composing a continuum robot of multiple segments. |

## Note
The backbone of a continuum robot does not necessarily have to be continuous. The biological counterpart, e.g. snakes, have a continuous external appearance, but are vertebrates with an internal segmented backbone comprised of many very short rigid-links.

A similar paradigm can be applied to compose a discrete continuum robot. As in a serial robot arm, this can be achieved by concatenating multiple links connected by revolute joints. By keeping the link length short, the appearance of such a serial robot arm is resembling a continuous structure. In robotics, this type of robot is commonly referred to as a hyper-redundant robot, as it exhibits a high number of degrees of freedom in joint space. Those highly hyper-redundant robots can also be referred to as quasi-continuous or pseudocontinuum.
