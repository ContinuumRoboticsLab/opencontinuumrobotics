---
title: "Continuum Robots @ICRA23"
author: jbk
toc: true
category: research
excerpt: A curated list of continuum robotics research presented #ICRA2023.
header:
  teaser: /assets/images/posts/research/icra2023-teaser.jpg
---
This year's [IEEE International Conference on Robotics and Automation](https://www.icra2023.org) holds a firework of continuum robotics research! Are you getting ready for the conference and creating your itineary? The following presentations, workshops, and papers are on my list this year. You can find the full conference [program](https://ras.papercept.net/conferences/conferences/ICRA23/program) online!

## Keynotes
My keynote presentation at this year's ICRA is all about the [Open Continuum Robotics Project](https://www.opencontinuumrobotics.com). 

### Accelerating Medical Robotics Innovation with the Open Continuum Robotics Project
Tuesday, 17:00 - 18:30 - Healthcare Robotics
{: .notice}

**Speaker:** Jessica Burgner-Kahrs

**Abstract:** From robotically steered catheters and bronchoscopes to single port flexible instruments, continuum robotics has led to great advances in medical robotics over the past decade. Yet, research findings remain stubbornly difficult to reproduce because continuum robotics hardware and software are not readily available, and no common systems exist. Ultimately this slows the pace of innovation.

The Open Continuum Robotics Project combines hardware, software, and education with the goal of fostering more collaborative, cost-effective, and reproducible research. This enables rapid prototyping and iterative design, allowing researchers and clinicians to test and refine their ideas more quickly – including in resource-constrained settings. In this way, the Open Continuum Robotics Project accelerates the development of new technologies and treatments in medical robotics.


## Workshop and Tutorials
ICRA 2023 features an incredible rich set of workshops and tutorials this year, which makes it very hard to choose which one to attend (or when to rush from one room to the next #FOMO). The following ones feature aspects of continuum robotics and are worth a look!

### Monday
- MW02: [Soft Growing Robots: From Search-and-Rescue to Intraluminal Interventions](https://www.growing-robots.com/)
- MW05: [Shrinking the Cutting Edge: Making Small-Scale Medical Robots for Humans](https://www.santannapisa.it/en/icra-2023-workshop-small-scale-medical-robots)
- MW10: [Origami-based structures for designing soft robots with new capabilities](https://www.origabot.cnrs.fr/workshop-icra-2023/)

### Friday
- FW12: [Geometric Representations: The Roles of Screw Theory, Lie algebra, & Geometric Algebra](https://www.mirmi.tum.de/mirmi/events/icra-2023-workshop/)
- FW16: [Soft Robotics: Fusing function with structure](https://soft-robotics-workshop.bitbucket.io)
- FW22: [Force and shape perception for surgical instruments and robots](https://sites.google.com/view/icra2023ws-force-shape/home)
- FT29: [Towards an accessible soft robotics toolbox and validation test rig](http://www.softrobotictoolbox.org)

## Talks
The majority of oral presentations of ICRA 2023 are adressing continuum robot modeling, with a focus on kinetostatics and dynamics using Cosserat theory and optimal control theory. It is fantastic to see a trend towards open toolboxes and knowledge mobilization! There are also some exciting soft continuum robot designs!

###  FEA-Based Soft Robotic Modeling: Simulating a Soft-Actuator in SOFA (I)
09:50-10:00, Paper TuAT2.9
{: .notice}

**Authors:** Ferrentino, Pasquale; Roels, Ellen; Brancart, Joost; Terryn, Seppe	; Van Assche, Guy; Vanderborght, Bram

**Abstract:** Soft robotics modeling is a research topic that is evolving fast. Many techniques are present in literature but most of them require analytical models with a lot of equations that are time-consuming, hard to resolve, and not so easy to handle. For this reason, the help of a soft mechanics simulator is essential in this field. In fact, this paper presents a tutorial on how to build a soft-robot model using an open-source Finite Element Analysis (FEA) simulator, called SOFA. This software is able to generate a simulation scene from a code written in Python or XML, so it can be used by people that with different fields of competence like mechanical knowledge, knowledge of material properties and programming skills. As a case study, a Python simulation of a cable-driven soft actuator that makes contact with a rigid object is considered. The basic working principles of SOFA required to make a scene are explained step by step. In particular, it shows how to simulate the mechanics and animate the bending behavior of the actuator. Furthermore, it will be shown also how to retrieve and save data from simulation, demonstrating that SOFA can easily adapt to a multi-disciplinary subject as the research in soft-robotics, but also be useful for teaching simulation and programming language principles to engineering students.

### SoRoSim: A MATLAB Toolbox for Hybrid Rigid-Soft Robots Based on the Geometric Variable-Strain Approach (I)
15:40-15:50, Paper TuBT2.5
{: .notice}

**Authors:** Mathew, Anup Teejo; Ben Hmida, Ikhlas; Armanini, Costanza; Boyer, Frédéric; Renda, Federico

**Abstract:** Soft robotics has been a trending topic within the robotics community for almost two decades. However, available tools for the modeling and analysis of soft robots are still limited. This paper introduces a user-friendly MATLAB toolbox, SoRoSim, that integrates the Geometric Variable Strain model of Cosserat rods to facilitate the static and dynamic analysis of soft, rigid, or hybrid robotic systems. We present a brief overview of the design and structure of the toolbox and validate it by comparing its results with those published in the literature. To highlight the toolbox's potential to efficiently model, simulate, optimize, and control various robotic systems, we demonstrate four sample applications. The demonstrated applications explore different actuator and external loading conditions of single-, branched-, open-, and closed-chain robotic systems. We think that the soft-robotics research community will significantly benefit from the SoRoSim toolbox for a wide variety of applications.

### A Geometrically-Exact Assumed Strain Modes Approach for the Geometrico and Kinemato-Static Modellings of Continuum Parallel Robots (I)
15:50-16:00, Paper TuBT2.6
{: .notice}

**Authors:** Briot, Sébastien; Boyer, Frédéric

**Abstract:** There is a growing interest on the study of continuum parallel robots (CPRs) due to their higher stiffness and better dynamics capacities than serial continuum robots (SCRs). Several works have focused on the computation of their geometrico- and kinemato-static models, that can be sorted into two main categories: (i) models based on the continuous Cosserat equations: They are very accurate but assessing elastic stability with them is tricky; (ii) discretized models: They allow easily checking the elastic stability but they require a large number of elastic variables to be accurate.
In this paper, we extend an approach based on assumed strain modes developed for the dynamics of SCRs to the statics of CPRs. This method is able to predict the robot configuration with an excellent accuracy with a very limited number of elastic variables, contrary to other discretization methods. The method is also more than 100 times faster than finite differences for a better prediction accuracy. Finally, it is possible to assess the robot elastic stability by only checking the Hessian of the potential energy as for any discretization method, thus making the analysis of this property simpler.

### Towards a Physics-Based Model for Steerable Eversion Growing Robots
16:00-16:10, Paper TuBT2.7
{: .notice}

**Authors:** Wu, Zicong; De Iturrate Reyzabal, Mikel; Sadati, Seyedmohammadhadi; Liu, Hongbin; Ourselin, Sebastien; Leff, Daniel Richard; Katzschmann, Robert Kevin; Rhode, Kawal; Bergeles, Christos

**Abstract:** Soft robots that grow through eversion/apical extension can effectively navigate fragile environments such as ducts and vessels inside the human body. This letter presents the physics based model of a miniature steerable eversion growing robot. We demonstrate the robot’s growing, steering, stiffening and interaction capabilities. The interaction between two robot-internal components is explored, i.e., a steerable catheter for robot tip orientation, and a growing sheath for robot elongation/retraction. The behavior of the growing robot under different inner pressures and external tip forces is investigated. Simulations are carried out within the SOFA framework. Extensive experimentation with a physical robot setup demonstrates agreement with the simulations. The comparison demonstrates a mean absolute error of 10–20% between simulation and experimental results for curvature values, including catheter-only experiments, sheath-only experiments and full system experiments. To our knowledge, this is the first work to explore physics-based modelling of a tendon-driven steerable eversion growing robot. While our work is motivated by early breast cancer detection through mammary duct inspection and uses our MAMMOBOT robot prototype, our approach is general and relevant to similar growing robots.

###  Statics and Dynamics of Continuum Robots Based on Cosserat Rods and Optimal Control Theories (I)
16:20-16:30, Paper TuBT2.9
{: .notice}

**Authors:** Boyer, Frédéric; Lebastard, Vincent; Candelier, Fabien; Renda, Federico; Alamir, Mazen

**Abstract:** This paper explores the relationship between optimal control and Cosserat beam theory from the perspective of solving the forward and inverse dynamics (and statics as a subcase) of continuous manipulators and snake-like bio-inspired locomotors. By invoking the principle of minimum potential energy, and the Gauss principle of least constraint, it is shown that the quasi-static and dynamic evolution of these robots, are solutions of optimal control problems (OCPs) in the space variable, which can be solved at each step (of loading or time) of a simulation with the shooting method. In addition to offering an alternative viewpoint on several simulation approaches proposed in the recent past, the optimal control viewpoint allows us to improve some of them while providing a better understanding of their numerical properties. The approach and its properties are illustrated through a set of numerical examples validated against a reference simulator.

### COBRA: From Industrial to Medical Surgery with Slender Continuum Robots (I)
15:00-15:10, Paper WeBT2.1
{: .notice}

**Authors:** Alatorre, David; Robles-Linares, Jose A.; Russo, Matteo; Elbanna, Mohamed A.; Wild, Samuel; Dong, Xin; Mohammad, Abdelkhalick; Kell, James; Norton, Andy; Axinte, Dragos

**Abstract:** The maintenance of critical industrial components is often hindered by limited access, tortuous passages, and complex geometries. In highly constrained environments, inspection tasks are currently performed with borescopes, but even skilled operators struggle with hard-to-reach targets and the limited mobility prevents in-situ repair when defects are identified. Thanks to an active shape control, snake-like and continuum robots can outperform borescopes for short range inspection as well as enable intervention. However, their actuation technology limits their scalability in length, as longer bodies pose control challenges due to their intrinsically low stiffness and space constraints. To overcome the limitations of both borescopes and continuum robots, we here propose a modular design at their intersection, with both active tendon-driven and passively flexible segments. The main elements of the novel design, including actuation and control interface, are described, and the system is demonstrated in scenarios for aerospace assets, nuclear installations, and robot-assisted surgery.

### A Generalized Framework for Concentric Tube Robot Design Using Gradient-Based Optimization (I)
10:10-10:20, Paper ThAT2.8
{: .notice}

**Authors:** Lin, Jui-Te;Girerd, Cedric; Yan, Jiayao; Hwang, John T.; Morimoto, Tania K.

**Abstract:** Concentric tube robots (CTRs) show particular promise for minimally invasive surgery due to their inherent compliance and ability to navigate in constrained environments. Due to variations in anatomy among patients and variations in task requirements among procedures, it is necessary to customize the design of these robots on a patient- or population-specific basis. However, the complex kinematics and large design space make the design problem challenging. Here we propose a computational framework that can efficiently optimize a robot design and a motion plan to enable safe navigation through the patient’s anatomy. The current framework is the first fully gradient-based method for CTR design optimization and motion planning, enabling an efficient and scalable solution for simultaneously optimizing continuous variables, even across multiple anatomies. The framework is demonstrated using two clinical examples, laryngoscopy and heart biopsy, where the optimization problems are solved for a single patient and across multiple patients, respectively.

### Magnetic Soft Continuum Robots with Braided Reinforcement
10:20-10:30, Paper ThAT2.9
{: .notice}

**Authors:** Lloyd, Peter Robert; Onaizah, Onaizah; Pittiglio, Giovanni; Chathuranga, Damith Suresh; Chandler, James Henry; Valdastri, Pietro

**Abstract:** Flexible catheters are used in a wide variety of surgical interventions including neurological, pancreatic and cardiovascular. In many cases a lack of dexterity and miniaturization along with excessive stiffness results in large regions of the anatomy being deemed inaccessible. Soft continuum robots have the potential to mitigate these issues. Due to its enormous potential for miniaturization, magnetic actuation is of particular interest in this field. Currently, flexible magnetic catheters often rely on forces of anatomical interaction to generate large deformations during navigation and for soft anatomical structures this could be considered potentially damaging. In this study we demonstrate the insertion of a high aspect ratio, 50 mm long by 2 mm diameter, soft magnetic catheter capable of navigating up to a 180 degree bend without the aid of interactive forces. This magnetic catheter is reinforced with a lengthwise braided structure and its magnetization allows it to shape form along tortuous paths. We demonstrate our innovation in a planar silicone pancreas phantom. We also compare our approach with a mechanically equivalent tip driven magnetic catheter and with an identically magnetized, unreinforced catheter.



###  Kinetostatic Modeling of Tendon-Driven Parallel Continuum Robots (I)
15:00-15:10, Paper ThBT5.1
{: .notice}

**Authors:** Lilge, Sven; Burgner-Kahrs, Jessica

**Abstract:** Tendon-driven parallel continuum robots consist of multiple individual continuous kinematic chains, that are actuated in bending utilizing tendons routed along their backbones. This work derives and proposes a Cosserat rod based kinetostatic modeling framework for such parallel structures that allows for efficiently solving the forward, inverse and velocity kinetostatic problems. Using this model, the kinematic properties such as reachable workspace, singularities, manipulability and compliance of tendon-driven parallel continuum robots are studied in detail. Experiments are conducted using a real robotic prototype to validate the derived modeling approach. Overall, a median pose accuracy of 4.9 mm, corresponding to 3.4% of the continuum robots’ lengths, and 6.2◦ is achieved. The median of the model’s computation time results in 0.51 s on standard computing hardware. Fast computations of below 100 ms can be achieved, if an appropriate initial guess for solving the kinetostatic model is available, making the model suitable for a range of different applications including optimization or control.

## Posters
The poster presentations at ICRA 2023 cover various aspects of (soft) continuum robots, including design, control, and sensing.

### A Soft Hybrid-Actuated Continuum Robot Based on Dual Origami Structures
08:30-10:10, Paper TuPO1S-01.2
{: .notice}

**Authors:** Tao, Jian; Hu, Qiqiang; Luo, Tianzhi; Dong, Erbao

**Abstract:** Soft continuum robots have shown tremendous potential for medical and industrial applications owing to their flexibility and continuous deformability. However, their telescopic and bending capabilities and variable stiffness are still limited. This study proposes a novel origami-inspired soft continuum robot to possess large telescopic and bending capabilities while improving stiffness based on the principle of antagonistic actuation. The soft robot consists of dual origami structures. The inner forms an air chamber actuated by pneumatics, and the outer is controlled by nine tendon-driven actuators. The proposed design uses the advantages of a hybrid actuation to achieve motion and stiffness control. The performance of the soft robot is studied experimentally based on single and three robot modules. Results show that the robot has an excellent stretch ratio and a maximum bending angle of 180°. The robot can also increase stiffness to resist the bending deformation induced by self-weight and loads.

### Image-Based Pose Estimation and Shape Reconstruction for Robot Manipulators and Soft, Continuum Robots Via Differentiable Rendering
Tuesday 08:30-10:10, Paper TuPO1S-01.6, Room T8
{: .notice}

**Authors:** Lu, Jingpei; Liu, Fei; Girerd, Cedric; Yip, Michael C.

**Abstract:** State estimation from measured data is crucial for robotic applications as autonomous systems rely on sensors to capture the motion and localize in the 3D world. Among sensors that are designed for measuring a robot's pose, or for soft robots, their shape, vision sensors are favorable because they are information-rich, easy to set up, and cost-effective. With recent advancements in computer vision, deep learning-based methods no longer require markers for identifying feature points on the robot. However, learning-based methods are data-hungry and hence not suitable for soft and prototyping robots, as building such bench-marking datasets is usually infeasible. In this work, we achieve image-based robot pose estimation and shape reconstruction from camera images. Our method requires no precise robot meshes, but rather utilizes a differentiable renderer and primitive shapes. It hence can be applied to robots for which CAD models might not be available or are crude. Our parameter estimation pipeline is fully differentiable. The robot shape and pose are estimated iteratively by back-propagating the image loss to update the parameters. We demonstrate that our method of using geometrical shape primitives can achieve high accuracy in shape reconstruction for a soft continuum robot and pose estimation for a robot manipulator.

###  Discrete-Time Model Based Control of Soft Manipulator with FBG Sensing
08:30-10:10, Paper TuPO1S-01.8
{: .notice}

**Authors:** Franco, Enrico; Aktas, Ayhan; Treratanakulchai, Shen; Garriga-Casanovas, Arnau; Donder, Abdulhamit; Rodriguez y Baena, Ferdinando

**Abstract:** In this article we investigate the discrete-time model based control of a planar soft continuum manipulator with proprioceptive sensing provided by fiber Bragg gratings. A control algorithm is designed with a discrete-time energy shaping approach which is extended to account for control-related lag of digital nature. A discrete-time nonlinear observer is employed to estimate the uncertain bending stiffness of the manipulator and to compensate constant matched disturbances. Simulations and experiments demonstrate the effectiveness of the controller compared to a continuous time implementation.

### A Soft Robot with Three Dimensional Shape Sensing and Contact Recognition Multi-Modal Sensing Via Tunable Soft Optical Sensors
08:30-10:10, Paper TuPO1S-02.1
{: .notice}

**Authors:** McCandless, Max; Juliá Wise, Frank; Russo, Sheila

**Abstract:** Soft optical sensing strategies are rapidly developing for soft robotic systems as a means to increase the controllability of soft compliant robots. In this paper, we present a roughness tuning strategy for the fabrication of soft optical sensors to achieve the dual functionality of shape sensing combined with contact recognition within a single multi-modal sensor. The molds used to fabricate the soft sensors are roughened via laser micromachining to achieve asymmetrical sensor responses when bent in opposite directions. We demonstrate the integration of these sensors into a fully soft robotic platform consisting of a multi-directional bending module with integrated 3D shape sensing and a gripper with tip position monitoring along with contact force recognition. We show the accuracy of our sensing strategy in validation experiments and a pick-andplace task is performed to demonstrate the robot’s functionality.

### On Tendon Driven Continuum Robots with Compressible Backbones
08:30-10:10, Paper TuPO1S-03.7
{: .notice}

**Authors:** Srivastava, Manu; Walker, Ian

**Abstract:** This paper discusses the effect of axial backbone compression on tendon-driven continuum robots. A new mechanics model for compensating for this effect that does not require tendon tension sensing or knowledge of manipulator material properties/stiffnesses is introduced and analyzed. In addition, we provide an analytical expression for the minimum preload on the tendons to achieve a given bend, a quantity determined empirically thus far. Our model is computationally efficient and achieves real time control on low cost hardware. The analysis is supported by experimental results demonstrating significant improvement over kinematics in open loop control of a tendon-driven continuum hose robot.

### Data-Driven Estimation of Forces Along the Backbone of Concentric Tube Continuum Robots
Tuesday 15:00-16:40, Paper TuPO2S-02.6, Room T8
{: .notice}

**Authors:** Donat, Heiko; Mohammadi, Pouya; Steil, Jochen J.

**Abstract:** Concentric tube continuum robots (CTCRs) belong to the family of continuum robots with applications in minimally invasive surgeries. Because of this application domain, measuring the external forces along the body of the robot is paramount. CTCRs are made up of thin elastic rods and are intended to be applied inside the human body, where conventional sensor-based measurements are not feasible. Consequently, research is resorting to estimate the forces through geometric, numeric, or optimization methods. However, these methods often suffer from slow convergence. In this paper, we introduce a novel data-driven approach for estimating contact forces along the body of a CTCR that offers an estimation precision comparable to the current state-of-the-art optimization-based approaches, but exhibits nearly two orders of magnitude faster convergence. The proposed method is scalable and exhibits a significant performance in response to a wide range of external forces. The approach was evaluated in simulations and on a real 2-tube CTCR.

### Modeling of a Robotic Transcatheter Delivery System
09:00-10:40, Paper WePO1S-01.6
{: .notice}

**Authors:** Nayar, Namrata Unnikrishnan; Qi, Ronghuai; Desai, Jaydev P.

**Abstract:** Intracardiac transcatheter systems guided by advanced imaging modalities are gaining popularity in treating mitral regurgitation in non-surgical candidates. Robotically steerable transcatheter systems must use model-based control strategies to ensure safer and more effective transcatheter procedures with less trauma while using smaller control gains. In this paper, a 4-DoF robotically steerable tendon-driven robot was fabricated, and the relationship between the tendon displacement and the joint angle was derived. This relation was derived in two parts to make this approach applicable to any other catheter system. A model was derived to determine the tendon tensions needed to achieve desired joint angles. Then, the tendon characteristics were studied, and a tendon elongation (TE) model was derived as a function of tendon length. Executing the modeling process in two steps makes it easy to introduce additional parameters like length, friction, and pose, to characterize complex systems like catheters. The TE model was used to actuate the joints of the robot and RMSE was computed to characterize its performance. Also, PID control was used along with the TE model to improve the system's performance, and the contribution of the model and the controller in the system was recorded.

### A Novel Concentric Tube Steerable Drilling Robot for Minimally Invasive Treatment of Spinal Tumors Using Cavity and U-Shape Drilling Techniques
09:00-10:40, Paper WePO1S-01.11
{: .notice}

**Authors:** Sharma, Susheela; Park, Ji Hwan; Amadio, Jordan P.; Khadem, Mohsen; Alambeigi, Farshid

**Abstract:** In this paper, we present the design, fabrication, and evaluation of a novel flexible, yet structurally strong, Concentric Tube Steerable Drilling Robot (CT-SDR) to improve minimally invasive treatment of spinal tumors. Inspired by concentric tube robots, the proposed two degree-of-freedom (DoF) CT-SDR, for the first time, not only allows a surgeon to intuitively and quickly drill smooth planar and out-of-plane J- and U- shape curved trajectories, but it also, enables drilling cavities through a hard tissue in a minimally invasive fashion. We successfully evaluated the performance and efficacy of the proposed CT-SDR in drilling various planar and out-of-plane J-shape branch, U-shape, and cavity drilling scenarios on simulated bone materials.

### Magnetic Ball Chain Robots for Endoluminal Interventions
09:00-10:40, Paper WePO1S-01.12
{: .notice}

**Authors:** Pittiglio, Giovanni; Mencattelli, Margherita; Dupont, Pierre

**Abstract:** This paper introduces a novel class of hyperredundant robots comprised of chains of permanently magnetized spheres enclosed in a cylindrical polymer skin. With their shape controlled using an externally-applied magnetic field, the spherical joints of these robots enable them to bend to very small radii of curvature. These robots can be used as steerable tips for endoluminal instruments. A kinematic model is derived based on minimizing magnetic and elastic potential energy. Simulation is used to demonstrate the enhanced steerability of these robots in comparison to magnetic soft continuum robots designed using either distributed or lumped magnetic material. Experiments are included to validate the model and to demonstrate the steering capability of ball chain robots in bifurcating channels.

### Model-Based Pose Estimation of Steerable Catheters under Bi-Plane Image Feedback
09:00-10:40, Paper WePO1S-03.2
{: .notice}

**Authors:** Lawson, Jared; Chitale, Rohan; Simaan, Nabil

**Abstract:** Small catheters undergo significant torsional deflections during endovascular interventions. A key challenge in enabling robot control of these catheters is the estimation of their bending planes. This paper considers approaches for estimating these bending planes based on bi-plane image feedback. The proposed approaches attempt to minimize error between either the direct (position-based) or instantaneous (velocity-based) kinematics with the reconstructed kinematics from bi-plane image feedback. A comparison between these methods is carried out on a setup using two cameras in lieu of a bi-plane fluoroscopy setup. The results show that the position-based approach is less susceptible to segmentation noise and works best when the segment is in a non-straight configuration. These results suggest that estimation of the bending planes can be accompanied with errors under 30◦. Considering that the torsional buildup of these catheters can be more than 180◦, we believe that this method can be used for catheter control with improved safety due to the reduction of this uncertainty.

### Image Segmentation for Continuum Robots from a Kinematic Prior
09:00-10:40, Paper WePO1S-03.4
{: .notice}

**Authors:** Watson, Connor; Nguyen, Anna; Morimoto, Tania K.

**Abstract:** In this work, we address the problem of robust segmentation of a continuum robot from images without the need for training data or markers. We present a method that leverages information about the kinematics of these robots to produce an estimate of the robot shape, which is refined through optimization over global image statistics. Our approach can be straightforwardly applied to any continuum robot design and is able to handle partial occlusions of the robot body, as well as challenging background conditions. We validate our method experimentally for a concentric tube robot in a simulated surgical environment and show that our method significantly outperforms a naive projection of the robot shape and color thresholding, which is commonly used in current vision-based estimation algorithms for these robots. Overall, this work has the potential to improve the viability of vision-based state estimation for continuum robots in real-world settings.

### An Equivalent Two Section Method for Calculating the Workspace of Multi-Segment Continuum Robots
09:00-10:40, Paper ThPO1S-12.4
{: .notice}

**Authors:** Fan, Yeman; Liu, Dikai

**Abstract:** Obtaining the shape and size of a robot’s workspace is essential for both its design and control. However, determining the accurate workspace of a multi-segment continuum robot by graphic or analytical methods is a challenging task due to its inherent flexibility and complex structure. Existing numerical methods have limitations when applied to a continuum robot. This paper presents an Equivalent Two Section (ETS) method for calculating the workspace of multi-segment continuum robots. This method is based on the forward kinematics and a piecewise constant curvature (PCC) model to determine the boundaries of the workspace. In order to verify the proposed method, simulation experiments are conducted using six different maximum bending angles and seven different number of segments. Results of the ETS method are compared to the true workspaces of these configurations estimated by an exhaustive approach. The results show that the proposed ETS method is both efficient and accurate, and has small estimation errors. Discussions on the advantages and limitations of the proposed ETS method are also presented.

### HaPPArray: Haptic Pneumatic Pouch Array for Feedback in Hand-Held Robots
15:00-16:40, Paper ThPO2S-23.1
{: .notice}

**Authors:** Luo, Xiaolei; Lin, Jui-Te; Morimoto, Tania K.

**Abstract:** Haptic feedback can provide operators of hand-held robots with active guidance during challenging tasks and with critical information on environment interactions. Yet for such haptic feedback to be effective, it must be lightweight, capable of integration into a hand-held form factor, and capable of displaying easily discernible cues. We present the design and evaluation of HaPPArray — a haptic pneumatic pouch array — where the pneumatic pouches can be actuated alone or in sequence to provide information to the user. A 3x3 array of pouches was integrated into a handle, representative of an interface for a hand-held robot. When actuated individually, users were able to correctly identify the pouch being actuated with 86% accuracy, and when actuated in sequence, users were able to correctly identify the associated direction cue with 89% accuracy. These results, along with a demonstration of how the direction cues can be used for haptic guidance of a medical robot, suggest that HaPPArray can be an effective approach for providing haptic feedback for hand-held robots.