---
title: "Tendon Routing Disks and their Effects on Motion Primitives"
author: jbk
toc: false
classes: wide
category: 101
excerpt: Let's conceptually think about tendon routing disks. They provide channels to route the tendon actuating a continuum robot.
header:
    teaser: /assets/images/posts/101-tendon-routing-teaser.jpg
---
We have looked into the general [motion primitives]({% post_url /2022-10-28-motion-primitives %}) in continuum robotics: spatial bending, twisting, extension/contraction. Today, we look at partially constrained tendon paths and how the design of tendon routing disk influences the motion capabilities.

Let's recap: When we first looked at [tendon-driven continuum robots]({% post_url /2022-11-11-tdcr-intro %}), we looked at the most general design, i.e. with tendon routing disks at equidistant spacing afixed to a a flexible backbone. Tendons terminate at the end disk of each segment to actuate it. Most generally, these tendons are routed in parallel to the central backbone. For spatial bending either 3 separate tendons or 2 antagonistic tendon pairs are used. To achieve a tendon-driven continuum robot segment capable of all motion primitive, we will expand our understanding of tendon routing disks and its implications. 

Let's conceptually think about tendon routing disks. They provide channels to route the tendon actuating a continuum robot.  We depict four conceptual tendon routing disk types below. The dotted arrows indicate the degree of freedom of the disks themselves and the solid arrows indicate the motion primitives achievable. We omit the tendon themselves.

![]({{ site.url }}{{ site.baseurl }}/assets/images/posts/101_FSD.jpg)

The most common type is afixed to a central backbone and routes the tendons with a fixed distance parallel to the backbone. We refer to this type of tendon routing disk as

**Type-0**
: A tendon routing disk which is fixed and can neither rotate nor translate along the backbone.

Fixing the tendon routing disks to the central backbone is the most restrictive as they only allow for bending. Allowing the tendon routing disks to freely translate along the central backbone allows for extension.

**Type-I**
: A translational spacer disk which can freely translate along the backbone but not rotate.

Most realizations of this tendon routing disk type ensure equidistant spacing of the disks as the backbone extends and contracts. This is either achieved by compression springs between disks or magnets within the disks alternating polarity for repulsion.

Conceptually, tendon routing disks may also be freely rotating about the central backbone, but constrained in position along the backbone. Such a tendon routing would enable bending but also twist as the tendon route is not constrained to being parallel.

**Type-II**
: A rotational space disk which can freely rotate about the backbone while translation is prohibited.

We fabricated a tendon-driven continuum robot segment using type-II disks. The end disk is rigidly attached to the backbone rod which can rotate about its axis. The base disk is fixed in orientation. The image series below  shows different rotation angles $\alpha$.

![image]({{ site.url }}{{ site.baseurl }}/assets/images/posts/101-type-ii-example.jpg)

Ultimately, the least restrictive tendon routing disk is free to rotate and translate along the central backbone. Consequently, the tendon routing can allow for parallel and non-parallel tendon paths for bending and twisting, while also allowing for extension.

**Type-III**
: A spacer disk which can translate along and rotate freely about the backbone.

Building on our extensible tendon-driven continuum robot design, we have fabricated a tendon-driven continuum robot segment with type-III disks. The image series below shows the prototype at various backbone rotation angles and applied tendon loads. The flag at the tip indicated the central backbone rotation angle. In addition to bending a twist can be observed. 
![image]({{ site.url }}{{ site.baseurl }}/assets/images/posts/101-type-iii-example.jpg)

The image series below shows the type-III tendon disk prototype contracting while also adjusting the rotation angle. 
![image]({{ site.url }}{{ site.baseurl }}/assets/images/posts/101-type-iii-extension-example.jpg)

**Further Reading**: You want to read more on tendon routing disk types and the prototypes shown above? Check out our open access paper in Frontiers in Robotics & AI[^Grassmann].
{: .notice--success}

## References

[^Grassmann]: R.M. Grassmann, P. Rao, Q. Peyron, J. Burgner-Kahrs: FAS—A Fully Actuated Segment for Tendon-Driven Continuum Robots. Frontiers in Robotocs and AI, 9:873446, 2022. doi: [10.3389/frobt.2022.873446](https://doi.org/10.3389/frobt.2022.873446)