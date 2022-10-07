---
title: "Continuum Robots @IROS22"
author: jbk
toc: true
category: research
excerpt: A curated list of continuum robotics research presented @IROS22.
header:
  teaser: /assets/images/posts/research/iros_2022_teaser.jpg
---
This year's [IEEE/RSJ International Conference on Intelligent Robots and Systems](https://iros2022.org) holds a firework of continuum robotics research! Getting ready for the conference and creating your itineary? We curated a list of papers and their presentations timeslotsç!

## Design

### Multiple Curvatures in a Tendon-Driven Continuum Robot Using a Novel Magnetic Locking Mechanism
Monday 10:40-10:50, Paper MoA-8.5
{: .notice}

**Authors:** Pogue, Chloe	and Rao, Priyanka	and Burgner-Kahrs, Jessica and Diller, Eric D. (University of Toronto); Peyron, Quentin	(INRIA); Kim, Jongwoo	(Kyung Hee University)

**Abstract:** Tendon-driven continuum robots show promise for use in surgical applications as they can assume complex configurations to navigate along tortuous paths. However, to achieve these complex robot shapes, multiple segments are required as each robot segment can bend only with a single constant curvature. To actuate these additional robot segments, multiple tendons must typically be added on-board the robot, complicating their integration, robot control, and actuation. This work presents a method of achieving two curvatures in a single tendon-driven continuum robot segment through use of a novel magnetic locking mechanism. Thus, the need for additional robot segments and actuating tendons is eliminated. The resulting two curvatures in a single segment are demonstrated in two and three dimensions. Furthermore, the maximum magnetic field required to actuate the locking mechanism for different robot bending angles is experimentally measured to be 6.1 mT. Additionally, the locking mechanism resists unintentional unlocking unless the robot assumes a 0° bending angle and a magnetic field of 18.1 mT is applied, conditions which are not typically reached during routine use of the system. Finally, addressable actuation of two locking mechanisms is achieved, demonstrating the capability of producing multiple curvatures in a single robot segment.

### Design of a Modular Continuum Robot with Alterable Compliance Using Tubular-Actuation
Monday 14:40-14:50, Paper MoB-8.4
{: .notice}

**Authors:** Wang, Mingyuan	and Du, Liang	and Bao, Sheng and Yuan, Jianjun and and Zhou, Jinshu	(Shanghai University); Ma, Shugen	(Ritsumeikan University)

**Abstract:** Compliance is good. However, it is challenging for one compliant continuum robot to finish both high precision manipulation and environmental-adapted motions. In this paper, a modular con-tinuum robot with the alterable compliance characteristic is pro-posed. Besides, an actuation module is also proposed using a tubular-screw mechanism for non-slippage transmission. Kine-matic analyses and dynamic co-simulation are performed to study the continuum robot. Furthermore, two potential applica-tion scenarios of pick-and-place manipulation and confined space navigating are carried out to demonstrate the advantages of the alterable compliance design. This study presents a capable con-tinuum robotic solution for non-structural inspection tasks, with potential for in-situ applications in restricted and hazardous en-vironments.

### A Geometric Design Approach for Continuum Robots by Piecewise Approximation of Free-Form Shapes
Tuesday 10:20-10:30, Paper TuA-14.3
{: .notice}

**Authors:** Wang, Sicheng and Blumenschein, Laura (Purdue University)

**Abstract:** As soft, continuum robots see increasing areas of application, many scenarios have arisen where it is necessary to consider the geometric shape of the robot. The current approaches to robot kinematics, such as the piecewise constant-curvature (PCC) model, are effective in representing simple overall robot geometry and estimating the end-effector state, but they are less intuitive for planing robots that involve complex geometries. In this work, we propose a solution to the geometric design problem by a two-part approach: a free-form spline defines a "shape curve" that describes the overall geometry of the robot, and then a "kinematic curve" composed of shapes that are feasible to replicate with continuum robots is fitted to the shape curve. As an implementation of this approach, we specifically explore the application of piecewise cubic Bezier curves in designing the shape curve of the robot, and pairs of arcs to construct the kinematic curves. Finally, the approach is applied to a tip-extension "vine" robot that is designed and fabricated to "grow" along a designed path and access the top surface of an obstacle.

### Design, Teleoperation Control and Experimental Validation of a Dexterous Robotic Flexible Endoscope for Laparoscopic Surgery
Tuesday 10:50-11:00, Paper TuA-OL1.6
{: .notice}

**Authors:** Ma, Xin	Chinese and Wang, Xuchen and Cao, Rui	and Au, K. W. Samuel (The Chinese University of Hong Kong)

**Abstract:** Existing robotic endoscopes for laparoscopic surgery, predominantly rigid or limited in dexterity, occupy a large motion space1. The large occupied motion space necessitates large incisions and reduces the motion space for surgeons to simultaneously operate other surgical instruments. Meanwhile, surgeons only have limited view adjustment capability to avoid occlusion and they often have to lift/push some organs to observe occluded target lesions in some operations such as cholecystectomy. The situation gets worse when the operations are on obese patients. In this paper, we develop a novel dexterous robotic flexible endoscope (DRFE), which is comprised of a concentric cable-driven structure and a 2-DoF articulated joint attached to the end of DRFE, for laparoscopic surgery. The proposed design occupies much less motion space both inside and outside human body as compared to conventional robotic flexible endoscopes. When used in surgery, the part of the endoscope outside the body can remain still, which reduces the risk of expanding the incision and simplifies the structure of the remote center mechanism. Simulation and experimental studies are performed to validate the effectiveness of the proposed device in the improvement of vision occlusion and usability. Initial results reveal that the DRFE is highly dexterous and accurate in observing lesions with vision occlusion.

### A Miniature Continuum Robot with Integrated Piezoelectric Beacon Transducers and Its Ultrasonic Shape Detection in Robot-Assisted Minimally Invasive Surgeries
Tuesday 1:00-11:10, Paper TuA-OL1.7
{: .notice}

**Authors:** Yin, Zhanpeng and Hong, Yan and Zhang, Yingxuan and Ju, Feng (Nanjing University of Aeronautics and Astronautics); Sun, Xiaoyu	and Shen, Zhiyuan	and Drinkwater, Bruce (University of Bristol)

**Abstract:** Minimally invasive surgeries (MIS) or natural orifice transluminal endoscopic surgeries (NOTES) such as the transurethral resection of bladder tumor (TURBT) require the surgical robot to be miniaturized to perform surgical procedures in confined spaces. However, the surgical robot’s tiny size poses problems in its fabrication and shape sensing. In this paper, a miniature continuum surgical robot is proposed with a unique laminated structure which can be fabricated through a 2D lamination process and converted into 3D through folding. This multi-material laminated structure also facilitates the integration of tiny piezoelectric transducers on the robot’s surface as beacons to generate ultrasonic waves for shape detection. A novel beacon total focusing method (b-TFM) algorithm is developed to process the received ultrasonic data and create a high-quality ultrasonic image from which the shape of the continuum robot can be extracted. The proposed robot and the ultrasonic shape detection method are validated through simulations and experiments. The error in the open-loop trajectory control is less than 4 mm without compensation, and the error in the ultrasonic shape detection is less than 1 mm. This confirms the possibility of improving the trajectory control accuracy by using the detected shape as a feedback for closed-loop control.

### Development of a 6 DOF Soft Robotic Manipulator with Integrated Sensing Skin
Tuesday 13:30-13:40, Paper TuB-14.7
{: .notice}

**Authors:** Treratanakulchai, Shen	and Franco, Enrico and 
Garriga-Casanovas, Arnau and Kassanos, Panagiotis and 
Rodriguez y Baena, Ferdinando (Imperial College); Hu, Minghao	(Delft University of Technology)

**Abstract:** This paper presents a new 6 DOF soft robotic manipulator intended for colorectal surgery. The manipulator, based on a novel design that employs an inextensible tube to limit axial extension, is shown to maximize the force exerted at its tip and the bending angle, the latter being measured with a soft sensing skin. Manufacturing of the prototype is achieved with a lost-wax silicone-casting technique. The kinematic model of the manipulator, its workspace, and its manipulability are discussed. The prototype is evaluated with extensive experiments, including pressure-deflection measurement with and without tip load, and lateral force measurements with and without the soft sensing skin to assess hysteresis. The experimental results indicate that the prototype fulfils the key design requirements for colorectal surgery: (i) it can generate sufficient force to perform a range of laparoscopic tasks; (ii) the workspace is commensurate with the dimensions of the large intestine; (iii) the soft sensing skin only results in a marginal reduction of the maximum tip rotation within the range of pressures and external loads relevant for the chosen application.

### Design and Experimental Characterization of a Push-Pull Flexible Rod-Driven Soft-Bodied Robot
Tuesday 15:20-15:30, Paper TuC-14.8
{: .notice}

**Authors:** Wang, Peiyi and Guo, Sheng (Beijing Jiaotong University); Tang, Zhiqiang	and Xin, Wenci and Laschi, Cecilia (National University of Singapore); Xie, Zhexin (Beihang University)

**Abstract:** Soft robots with a well-balanced performance in terms of dexterity, accuracy, and payload have a great potential for application. Balancing safe human-robot interaction with operation performance enables the use of soft robot in biomedical fields, among others, such as surgery, rehabilitation and elder care. In this letter, we present a rod-driven soft robot (RDSR) where the flexible rods embedded in the silicone-based body provide a double push-pull actuation, to satisfy the needs of balanced performance. The RDSR can realize multi DOFs movement with elongation, contraction and bending. For trajectory tracking, Gaussian process model enables RDSR to achieve more accurate motion control with an RMSE within 2.8mm compared to the constant curvature model with that within 10.8mm. Comparative experiments demonstrate that the workspace, vertical and lateral stiffness of the RDSR are up to 5, 2.6 and 5.2 times that of an analogous tendon-driven soft robot (TDSR), respectively. Additionally, the RDSR possesses the ability, that the TDSR does not have, to actively apply pushing perpendicular to an inclined plane. Based on numerical Jacobian matrix, the maximum force along target direction is greater than 4N for a 30° plane. Furthermore, pick-and-place tests validate that our soft robot, with large workspace, precise and steady motion, is capable of conducting object manipulation tasks.

### Shape Memory Polymer Variable Stiffness Magnetic Catheters with Hybrid Stiffness Control
Wednesday 11:20-11:30, Paper WeA-7.9
{: .notice}

**Authors:** Mattmann, Michael and Boehler, Quentin	and Chen, Xiang-Zhong and Pané, Salvador and Nelson, Bradley J. (ETH Zürich)

**Abstract:** Variable stiffness catheters typically rely on thermally induced stiffness transitions with a transition temperature above body temperature. This imposes considerable safety limitations for medical applications. In this work, we present a variable stiffness catheter using a hybrid control strategy capable of actively heating and actively cooling the catheter material. The proposed catheter is made of a single biocompatible shape memory polymer, which significantly increases its manufacturability and scalability compared to existing designs. Increased safety is obtained by ensuring a lower-risk compliant state at body temperature while maintaining higher stiffness ranges in actively controlled states. Additionally, the combined use of variable stiffness and magnetic actuation increases the dexterity and steerability of the device compared to existing robotic tools.

### Prismatic Soft Actuator Augments the Workspace of Soft Continuum Robots
Wednesday 17:10-17:20, Paper WeC-5.6
{: .notice}

**Authors:** Wand, Philipp and Fischer, Oliver and Katzschmann, Robert Kevin (ETH Zürich)

**Abstract:** Soft robots are promising for manipulation tasks thanks to their compliance, safety, and high degree of freedom. However, the commonly used bidirectional continuum segment design means soft robotic manipulators only function in a limited hemispherical workspace. This work increases a soft robotic arm's workspace by designing, fabricating, and controlling an additional soft prismatic actuator at the base of the soft arm. This actuator consists of pneumatic artificial muscles and a piston, making the actuator back-driveable. We increase the task space volume by 116%, and we are now able to perform manipulation tasks that were previously impossible for soft robots, such as picking and placing objects at different positions on a surface and grabbing an object out of a container. By combining a soft robotic arm with a prismatic joint, we greatly increase the usability of soft robots for object manipulation. This work promotes the use of integrated and modular soft robotic systems for practical manipulation applications in human-centered environments.

## Modeling 

### Towards Adaptive Continuous Control of Soft Robotic Manipulator Using Reinforcement Learning
Tuesday 13:20-13:30, Paper TuB-16.6
{: .notice}
**Authors:** Li, Yingqi and Wang, Xiaomei and Kwok, Ka-Wai (University of Hong Kong)

**Abstract:** Although the soft robot is gaining considerable popularity in dexterous and safe manipulation, accurate motion control is still an open problem to be explored. Recent investigations suggest that reinforcement learning (RL) is a promising solution but lacks efficient adaptability for Sim2Real transfer or environment variations. In this paper, we present a deep deterministic policy gradient (DDPG)-based control system for the continuous task-space manipulation of soft robots. Domain randomization is adopted in simulation for fast control-policy initialization, while an offline retraining strategy is utilized to update the controller parameters for incremental learning. The experiments demonstrate that the proposed RL controller can track a moving target accurately (with RMSE of 1.26 mm), and accommodate to external varying load effectively (with ~30% RMSE reduction after retraining). Comparisons among the proposed RL controller and other supervised-learning-based controllers in handling additional tip load were also conducted. The results support that our RL method is appropriate for automatic learning such that there is no need of manual interference for data processing, particularly in cases with external disturbances and actuation redundancy.

### Physics-Informed Recurrent Neural Networks for Soft Pneumatic Actuators
Tuesday 15:10-15:20, Paper TuC-14.7
{: .notice}

**Authors:** Sun, Wentao and Akashi, Nozomi	and Kuniyoshi, Yasuo and Nakajima, Kohei (University of Tokyo)

**Abstract:** Replacing sensors with indirect sensing techniques contributes to retaining the flexibility of soft robots. By combining physical models with recurrent neural networks (which we term a physics informed recurrent neural network [PIRNN] approach), we implemented a hybrid prediction scheme on two typical soft pneumatic actuators: a McKibben pneumatic artificial muscle and a pneumatic-based soft finger made of silicone. The results showed that this hybrid scheme robustly enhanced the prediction accuracy to a great extent, even when combined with an inaccurate physical model. We also present the broad applicability of the PIRNN approach, showing its effectiveness for diverse types of RNNs and soft robotics platforms. Our work fills the gaps in the literature by applying a physics-informed machine-learning approach to practical engineering problems in soft robotics.

### A Simulation Framework for Magnetic Continuum Robots
Tuesday 15:30-15:40, Paper TuC-9.9
{: .notice}

**Authors:** Dreyfus, Roland and Boehler, Quentin and Nelson, Bradley J. (ETH Zürich)

**Abstract:** Remote magnetic navigation is a technology used to robotically steer magnetic medical instruments, such as magnetic catheters and guidewires, for minimally invasive surgery. The ability to model and simulate the behavior of these magnetic instruments in complex anatomies is important for their clinical use in many ways. Simulation frameworks can improve their design, characterization, and automatic control capabilities, as well as provide training simulators for physicians. In this work we introduce a new simulation framework that accounts for both magnetic actuation and in- teractions forces with meshed collision models. The simulations are validated experimentally in 2d rigid models using a state-of- the-art electromagnetic navigation system. We also demonstrate the use of our framework to build training simulators for two endovascular navigation tasks including the exploration of the aortic arch and the internal carotid artery.

### Towards Accurate Modeling of Modular Soft Pneumatic Robots: From Volume FEM to Cosserat Rod
Wednesday 10:00-10:10, Paper WeA-5.1
{: .notice}

**Authors:** Wiese, Mats and Cao, Benjamin-Hieu	and Raatz, Annika (Leibniz Universität Hannover)

**Abstract:** Compared to their rigid counterparts, soft material robotic systems offer great advantages when it comes to flexibility and adaptability. Despite their advantages, modeling of soft systems is still a challenging task, due to the continuous and often highly nonlinear nature of deformation these systems exhibit. Tasks like motion planning or design optimization of soft robots require computationally cheap models of the system’s behavior. In this paper we address this need by deriving operational point dependent Cosserat rod models from detailed volume finite element models (FEM). While the latter offer detailed simulations, they generally come with high computational burden that hinders them from being used in time critical model-based methods like motion planning or control. Basic Cosserat rod models promise to provide computationally efficient mechanical models of soft continuum robots. By using a detailed FE model in an offline stage to identify operational point dependent Cosserat rod models, we bring together the accuracy of volumetric FEM with the efficiency of Cosserat rod models. We apply the approach to a fiber reinforced soft pneumatic bending actuator module (SPA module) and evaluate the model’s predictive capabilities for a single module as well as a two-module robot.

### A Dataset and Benchmark for Learning the Kinematics of Concentric Tube Continuum Robots
Wednesday 10:30-10:40, Paper WeA-7.4
{: .notice}

**Authors:** Grassmann, Reinhard M.	and Chen, Ryan Zeyuan	and Liang, Nan and Burgner-Kahrs, Jessica (University of Toronto)

**Abstract:** Establishing a physics-based model capturing the kinetostatic behavior of concentric tube continuum robots is challenging as elastic interactions between the flexible tubes constituting the robot result in a highly non-linear problem. The Goldstandard physics-based model using the Cosserat theory of elastic rods achieves reasonable approximations with 1.5-3% with respect to the robot's length, if well-calibrated. Learning-based models of concentric tube continuum robots have been shown to outperform the Goldstandard model with approximation errors below 1%. Yet, the merits of learning-based models remain largely unexplored as no common dataset and benchmark exist.

In this paper, we present a dataset captured from a three-tube concentric tube continuum robot for use in learning-based kinematics research. The dataset consists of 100,000 joint configurations and the corresponding four 6 dof sensors in SE(3) measured with an electromagnetic tracking system (github.com/ContinuumRoboticsLab/CRL-Dataset-CTCR-Pose). With our dataset, we empower the continuum robotics and machine learning community to advance the field. We share our insights and lessons learned on joint space representation, shape representation in task space, and sampling strategies. Furthermore, we provide benchmark results for learning the forward kinematics using a simple, shallow feedforward neural network. The benchmark results for the tip error are 0.74 mm w.r.t. position (0.4 % of total robot length) and 6.49 grad w.r.t. orientation.

### Nonlinear Dynamics Modeling and Fault Detection for a Soft Trunk Robot: An Adaptive NN-Based Approach
Wednesday 14:50-15:00, Paper WeB-5.2
{: .notice}

**Authors:** Zhang, Jingting and Chen, Xiaotian	and Stegagno, Paolo	and Yuan, Chengzhi (University of Rhode Island)

**Abstract:** This paper presents a radial basis function neural network (RBF NN) based methodology to investigate the dynamics modeling and fault detection (FD) problems for soft robots. Finite element method (FEM) is first used to derive a mathematical model to describe the dynamics of a soft trunk robot. An adaptive dynamics modeling approach is then designed based on this FEM model by incorporating model-reduction and RBF NN techniques. This approach is capable of achieving accurate identification of the soft robot’s highly-nonlinear dynamics, with the identified knowledge being obtained and stored in constant RBF NN models. Finally, a model-based FD scheme is proposed with the modeling results, which can achieve efficient FD for the soft robot whenever it encounters an unknown fault. Note that the proposed methods are generic and usable for general soft robots. Validation of these methods is performed through both computer simulation and physical experiments.

### Shape Representation and Modeling of Tendon-Driven Continuum Robots Using Euler Arc Splines
Wednesday 15:00-15:10, Paper WeB-5.3
{: .notice}

**Authors:** Rao, Priyanka and Peyron, Quentin and Burgner-Kahrs, Jessica (University of Toronto)

**Abstract:** Due to the compliance of tendon-driven continuum robots, carrying a load or experiencing a tip force result in variations in backbone curvature. While the spatial robot configuration theoretically needs an infinite number of parameters for exact description, it can be well approximated using Euler Arc Splines which use only six of them. In this letter, we first show the accuracy of this representation by fitting the Euler Arc splines directly to experimentally measured robot shapes. Additionally, we propose a 3D static model that can account for gravity, friction and tip forces. We demonstrate the utility of using efficient parameterization by analyzing the computation time of the proposed model and then, using it to propose a hybrid model that combines physics-based model with observed data. The average tip error for the Euler arc spline representation is 0.43% and the proposed static model is 3.25% w.r.t. robot length. The average computation time is 0.56 ms for nonplanar deformations for a robot with ten disks. The hybrid model reduces the maximum error predicted by the static model from 8.6% to 5.1% w.r.t. robot length, while using 30 observations for training.


## Sensing/State Estimation

### Environmental Interaction with Continuum Robots Exploiting Impact
Monday 16:30-16:40, Paper MoC-10.4
{: .notice}

**Authors:** Wooten, Michael and Walker, Ian (Clemson University)

**Abstract:** Continuum robots offer unique potential benefits for environmental exploration, notably in using their maneuverability to navigate congested environments. However, significant challenges remain in environmental sensing using continuum structures, within which space for local sensing is often extremely limited. In this paper, we discuss the use of novel impulsive interaction, i.e. active tapping, using continuum robots to sense and identify features within their environment. We introduce an impact model-based tapping approach for environmental feature detection with continuum robots which does not require the addition of specialized sensors, and demonstrate its utility in hardware. We contrast the method to two alternative approaches to contact detection. The methods are compared empirically on two different types of continuum robot hardware, the pneumatically actuated "OctArm" and a tendon actuated "Tendril". The results identify relative strengths of the approaches. The impact model based approach is shown to include information not accessible to the other approaches.

### Tactile Perception for Growing Robots Via Discrete Curvature Measurements
Monday 16:50-17:00, Paper MoC-19.6
{: .notice}

**Authors:** Bryant, Micah and Watson, Connor	and Morimoto, Tania K. (University of California, San Diego)

**Abstract:** Soft, growing robots have the ability to conform to their environment and traverse highly curved paths that would typically prove challenging for other robot designs. As they navigate through these constrained and cluttered environments, there is often significant interaction between the robot and its surroundings. In this work, we propose a method to enable tactile perception for growing robots, which utilizes commercially available, flexible sensors that measure the curvature of the robot shape at multiple locations. Our method consists of both a pouch design to enable seamless integration of the sensors with the material of the growing robot, as well as an algorithm for determining the location of point contacts along the robot body. We validate our proposed approach experimentally using a 3.5 cm robot that can grow to be 53 cm long. We show that we can localize a force applied to various locations along its length with an average error of 3.44±1.38 cm when the robot is unactuated and 4.62±0.95 cm when the robot is actuated. Additionally, we characterize the minimum distance required for our tactile sensing approach to discriminate between two separate contact points along the robot body to be 23.5 cm. Finally, we apply our method to a growing robot exploring an unknown environment and show that we are able to effectively determine when and where the growing robot collides with an unknown obstacle.

### Contact Localization of Continuum and Flexible Robot Using Data-Driven Approach
Wednesday 10:50-11:00, Paper WeA-7.6
{: .notice}

**Authors:** Ha, Xuan Thao and Wu, Di	and Borghesan, Gianni and Vander Poorten, Emmanuel B (KU Leuven); Lai, Chun-Feng	(Delft University of Technology); Ourak, Mouloud	(University of Leuven); Menciassi, Arianna	(Scuola Superiore Sant'Anna)

**Abstract:** Continuum robots such as robotic catheters are increasingly being used in minimally invasive surgery. Compliance contributes to enhanced safety during e.g. catheter insertion, however, estimation of contact force and location may help clinicians avoiding exerting excessive force. Ultimately this could lead to faster and safer interventions. Researchers proposed force sensors integrated in the catheter tip in the past. However, such sensors add extra complexity to the catheter design. Also, tip force sensors do not provide insights on forces that act along the catheter length. This paper proposes a data-driven approach for localizing contact forces that appear over the length of the catheter. The proposed approach consists of a collision detection method and a contact localization method. The framework only requires the measurement of the catheter's shape which can be done by an embedded multi-core Fiber Bragg Grating fiber. The method was validated experimentally with a 3D-printed continuum robot with an integrated multi-core fiber. A second contact localization method which is based on identifying the discontinuity in the measured curvature, is also implemented and compared with the proposed method. The static and dynamic experiments show a mean average localization error of 2.3 mm and 4.3 mm which correspond to respectively 3.3% and 6.1% of a 70 mm long flexible robot. These findings demonstrate that the proposed framework outperforms the previous methods and yields promising results. The contact state estimation algorithm can detect collisions in at most approximately 1.08s.

### Shape Reconstruction of Soft Manipulators Using Vision and IMU Feedback
Wednesday 11:00-11:10, Paper WeA-14.7
{: .notice}

**Authors:** Bezawada, Harish and Vikas, Vishesh and Woods, Cole (University of Alabama)

**Abstract:**  In recent times, soft manipulators have gardened immense interest given their dexterous abilities. A critical aspect for their feedback control involves the reconstruction of the manipulator shape. The research, for the first time, presents shape reconstruction of a soft manipulator through sensor fusion of information available from Inertial Measurement Units (IMUs) and visual tracking. The manipulator is modeled using multi-segment continuous curvature Pythagorean Hodograph (PH) curves. PH curves are a class of continuous curvature curves with an analytical expression for the hodograph (slope). The shape reconstruction is formulated as an optimization problem that minimizes bending energy of the curve with a length constraint and the information from IMUs and/or visual markers. The paper experimentally investigates the robustness of shape reconstruction for scenarios when position of all visual markers, or slope at all the knots (placement of sensors) are known. Occlusion of manipulator segments is frequent, hence, this scenario is simulated by fusing information of available slopes (IMUs) at all knots and position (vision) at some knots. The experiments are performed on a planar tensegrity manipulator with IMUs feedback and visual tracking. The robustness study indicates reliability of these models for real world applications. Additionally, the proposed sensor fusion algorithm provides promising results where, for most cases, the shape estimates benefit from additional position information. Finally, the low dimensionality of the optimization problem argues for extension of the approach for real-time applications.
 
### FBG-Based Variable-Length Estimation for Shape Sensing of Extensible Soft Robotic Manipulators
Wednesday 11:10-11:20, Paper WeA-14.8
 {: .notice}

**Authors:** Lu, Yiang and Chen, Wei and Chen, Zhi and Zhou, Jianshu and Liu, Yunhui (The Chinese University of Hong Kong)

**Abstract:** In this paper, we propose a novel variable-length estimation approach for shape sensing of extensible soft robots utilizing fiber Bragg gratings (FBGs). Shape reconstruction from FBG sensors has been increasingly developed for soft robots, while the narrow stretching range of FBG fiber makes it difficult to acquire accurate sensing results for extensible robots. Towards this limitation, we newly introduce an FBG-based length sensor by leveraging a rigid curved channel, through which FBGs are allowed to slide within the robot following its body extension/compression, hence we can search and match the FBGs with specific constant curvature in the fiber to determine the effective length. From the fusion with the above measurements, a model-free filtering technique is accordingly presented for simultaneous calibration of a variable-length model and temporally continuous length estimation of the robot, enabling its accurate shape sensing using solely FBGs. The performances of the proposed method have been experimentally evaluated on an extensible soft robot equipped with an FBG fiber in both free and unstructured environments. The results concerning dynamic accuracy and robustness of length estimation and shape sensing demonstrate the effectiveness of our approach.

### A Proprioceptive Method for Soft Robots Using Inertial Measurement Units
Wednesday 10:10-10:20, Paper WeA-5.2
{: .notice}

**Authors:** Martin, Yves J. and Bruder, Daniel	and Wood, Robert (Harvard University)

**Abstract:** Proprioception, or the perception of the configuration of one's body, is challenging to achieve with soft robots due to their infinite degrees of freedom and incompatibility with most off-the-shelf sensors. This work explores the use of inertial measurement units (IMUs), sensors that output orientation with respect to the direction of gravity, to achieve soft robot proprioception. A simple method for estimating the shape of a soft continuum robot arm from IMUs mounted along the arm is presented. The approach approximates a soft arm as a serial chain of rigid links, where the orientation of each link is given by the output of an IMU or by spherical linear interpolation of the output of adjacent IMUs. In experiments conducted on a 660mm long real-world soft arm, this approach provided estimates of its end effector position with a median error of less than 10% of the arm's length. This demonstrates the potential of IMUs to serve as inexpensive off-the-shelf sensors for soft robot proprioception.

### Model-Based Contact Detection and Accommodation for Soft Bending Actuators: An Integrated Direct/Indirect Adaptive Robust Approach
Wednesday 10:20-10:30, Paper WeA-5.3
{: .notice}

**Authors:** Hu, Yu	and Chen, Cong and Zou, Jun (Zhejiang University)

**Abstract:** Soft robots have intrinsic advantages in interaction with humans or complex environments for actual applications, during which various external disturbances (e.g., external contact or collision) are inevitable. They show remarkable abilities in complicated tasks due to their easily deformable bodies and compliance characteristic, while also bringing challenges to the modeling, control, and trajectory planning in precise tasks. Thereby, perception and reaction to external disturbances are quite critical. In this paper, we focus on the slowly varying external contact and propose a contact detection method for the fiber-reinforced soft bending actuator (FRSBA), which is based on the system dynamical behavior. When contact is detected, a parameter extension method is introduced to modify the dynamic model. Then, a backstepping-based integrated direct/indirect adaptive robust controller with contact detection and accommodation strategy (CDA-DIARC) is designed to deal with system nonlinearities, uncertainties, and parametric variations caused by the external contact. Theoretical proof and physical experiments validate the convergence and high trajectory tracking performance of the proposed methods under different contact environments.

### 3D Curvature-Based Tip Load Estimation for Continuum Robots
Wednesday 15:20-15:30, Paper WeB-14.5
{: .notice}

**Authors:** Diezinger, Matyas André and Tamadazte, Brahim and Laurent, Guillaume J. (Université Bourgogne Franche-Comté, Femto-St)

**Abstract:** This letter presents a method intended for the estimation of external force and moment applied at the tip of thin rods using vision-based shape measurements, with a view to be applied on continuum robots. A versatile vision process is developed that does not require any additional markers nor sensors to provide an accurate tri-dimensional reconstruction of the deformable rod shape. Then, the tip loads (i.e., forces and moments) are directly deduced from the curvature along this curve formed by deformed rod thanks to the resolution of a linear system without requiring any iterative optimization. The curvature is determined with a robust method that allows filtering out measurement noise and artifacts. Simulations show that this approach gives fast and precise results in both 2D (planar forces estimation without torsion) and 3D (spatial forces estimation). Experimental results on cantilever rods demonstrate an accuracy of 2.2% and 2.7% of the applied forces and moments, respectively.

### Estimating Forces Along Continuum Robots
Wednesday 15:50-16:00, Paper WeB-5.8
{: .notice}

**Authors:** Aloi, Vincent and Dang, Khoa and Rucker, Caleb (University of Tennessee); Barth, Eric J.	(Vanderbilt University)

**Abstract:** Continuum robots can be slender and flexible to navigate through complex environments, such as passageways in the human body. In order to control the forces that continuum robots apply during navigation and manipulation, we would like to detect the location, direction, and magnitude of contact forces distributions as they arise. In this paper, we present a model-based framework for sensing distributed loads along continuum robots. Using sensed positions along the robot, we use a nonlinear optimization algorithm to estimate the loading which fits the model-predicted robot shape to the data. We propose that Gaussian load distributions provide a seamless way to account for a wide range of loadings, including approximate point loads and uniform distributed loads, while avoiding the ill-conditioning associated with highly resolved force distributions. In addition, we gain computational efficiency by re-framing the problem as unconstrained weighted least-squares minimization and by solving this problem with an Extended Kalman-filter framework. We validate the approach on two prototype tendon-driven continuum robots in multiple 3D loading scenarios, displaying a mean error of 0.58 N in load magnitude and 7% mean error in load location with respect to the length of the respective robot.

### Continuum-Body-Pose Estimation from Partial Sensor Information Using Recurrent Neural Networks
Wednesday 16:20-16:30, Paper WeC-5.1
{: .notice}

**Authors:** Tanaka, Kazutoshi(OMRON SINIC X Corporation); Minami, Yuna	and Tokudome, Yuji and Inoue, Katsuma	and
Kuniyoshi, Yasuo and Nakajima, Kohei (University of Tokyo)

**Abstract:** Soft continuum arms have significant potential for use in various applications due to their extremely high degrees of freedom. For example, these soft arms can be used for grasping and manipulating fragile materials in the deep sea or carrying a human to rescue in unstructured environments. However, in these situations, the environment is often dark and visual cues are not always usable. Therefore, these arms must estimate their pose from proprioceptive sensors to control their behavior and execute their tasks in dark places. Estimating the pose in a dynamic situation is still challenging because of the arms' high dimensionality and the complex structural changes in the body shape. Therefore, this study demonstrates a novel method for estimating the pose of proprioceptive bending sensors using recurrent neural networks (RNNs). In particular, an RNN framework known as deep reservoir computing was used for this purpose. Results from experiments using an octopus-inspired soft robotic arm clearly indicate that the proposed method significantly outperforms existing methods using long short-term memory models or linear models. We expect that our proposed method will enable behavioral control of these arms in dark places such as the deep sea, space, and inside the human body in future applications.

## Motion Planning

### Equilibrium Manipulation Planning for a Soft Elastic Rod Considering an External Distributed Force and Intrinsic Curvature
Tuesday 13:50-14:00, Paper TuB-14.9
{: .notice}

**Authors:** Wu, Shirui	and Zhang, Jiwen and Wu, Dan (Tsinghua University)

**Abstract:** Previous work has shown that the set of equilibrium shapes of a rod is a smooth 6-dimensional manifold. We develop the Kirchhoff rod model in a differential equation form using Darboux vector that easily adds distributed force and intrinsic curvature. It can be seen that in this form, the manifold of the equilibrium set is the same. Furthermore, we address the rod manipulation planning problem which has the certain point on rod following a predefined spatial track. We propose a novel rod manipulation planning algorithm that considers the spatial configuration distance between the current and the goal, and follows its quickest descent direction in each planning step. The experiments show that it has a much higher successful rate than straight-line path planning in the Euclidean space of the gripper and significantly less planning time than the commonly used sampling method. The hardware experiments are also conducted on a platform that consists of a manipulator, an F/T sensor and two cameras. We choose soft rubber rods in the experiments, and the results validate the proposed model and methods.

### RRT*-Based Path Planning for Continuum Arms
Tuesday 15:00-15:10, Paper TuC-18.6
{: .notice}

**Authors:** Meng, Brandon	and Godage, Isuru S.	and Kanj, Iyad (DePaul University)

**Abstract:** Continuum arms are bio-inspired devices that exhibit continuous, smooth bending and generate motion through structural deformation. Rapidly-exploring random trees (RRT) is a traditional approach for performing efficient path planning. RRT approaches are usually based on exploring the configuration space (C-Space) of the robot to find a desirable work space (W-Space) path. Due to the complex kinematics and the highly non-linear mapping between the C-Space and W-Space of continuum arms, a high-quality path in the C-Space (e.g., a linear path) may not correspond to a desirable path/movement in the W-Space. Consequently, the C-Space RRT approaches that are based on C-Space cost functions do not lead to reliable and effective path planning when applied to continuum arms. In this paper, we propose a RRT* path planning approach for continuum arms that is based on exploring the W-Space of the robot as opposed to its C-Space. We show the successful applications of the proposed W-Space RRT* path planner in performing path planning with obstacle avoidance and in performing trajectory tracking. In all the aforementioned tasks, the quality of the paths generated by the proposed planner is superior to that of previous approaches and to its counterpart C-Space based RRT* approach, while the paths are generated in substantially less time.

### Contact-Implicit Trajectory and Grasp Planning for Soft Continuum Manipulators
Wednesday 10:40-10:50, Paper WeA-5.5
{: .notice}

**Authors:** Graule, Moritz A. and Teeple, Clark and Wood, Robert (Harvard University)

**Abstract:** As robots begin to move from structured industrial environments to the real world, they must be equipped to not only safely interact with the environment, but also reason about how to leverage contact to perform tasks. In this work, we develop a modeling and motion planning framework for continuum robots that accounts for contact anywhere along the robot. We first present an analytical model for continuum manipulators under contact and discuss the ideal choice of generalized coordinates given properties of the manipulator and task specifications. We then demonstrate the utility of our model by developing a motion planning framework that can solve a diverse set of tasks. We apply our framework to end effector path planning for a soft arm in an obstacle-rich environment, and grasp planning for soft robotic grippers, where contact can happen anywhere on the arm or gripper. Finally, we verify the utility of our model and planning framework by planning a grasp with a desired contact force for a soft antipodal gripper and testing this grasp in a hardware demonstration. Overall, our model and planning approach further enhance soft and continuum robots where they already excel: utilizing contact with the world to achieve their goals with a gentle touch.

## Control

### Autonomous Intraluminal Navigation of a Soft Robot Using Deep-Learning-Based Visual Servoing
Tuesday 13:40-13:50, Paper TuB-14.8
{: .notice}

**Authors:** Lazo, Joge F. and Ferrigno, Giancarlo and De Momi, Elena (Politecnico Di Milano); Lai, Chun-Feng	and Breedveld, Paul and 
Dankelman, Jenny (TU Delft); Moccia, Sara	(Scuola Superiore Sant'Anna); Rosa, Benoît (CNRS); Catellani, Michele	(European Institute of Oncology); de Mathelin, Michel	(University of Strasbourg)

**Abstract:** Navigation inside luminal organs is an arduous task that requires non-intuitive coordination between the movement of the operator's hand and the information obtained from the endoscopic video. The development of tools to automate certain tasks could alleviate the physical and mental load of doctors during interventions, allowing them to focus on diagnosis and decision-making tasks. In this paper, we present a synergic solution for intraluminal navigation consisting of a 3D printed endoscopic soft robot that can move safely inside luminal structures. Visual servoing, based on Convolutional Neural Networks(CNNs) is used to achieve the autonomous navigation task. The CNN is trained with phantoms and in-vivo data to segment the lumen, and a model-less approach is presented to control the movement in constrained environments. The proposed robot is validated in anatomical phantoms in different path configurations. We analyze the movement of the robot using different metrics such as task completion time, smoothness, error in the steady-state, mean and maximum error. We show that our method is suitable to navigate safely in hollow environments and conditions which are different than the ones the network was originally trained on.

### A Unified and Modular Model Predictive Control Framework for Soft Continuum Manipulators under Internal and External Constraints
Wednesday 10:30-10:40, Paper WeA-5.4
{: .notice}

**Authors:** Spinelli, Filippo Alberto and Katzschmann, Robert Kevin (ETH Zürich)

**Abstract:** luidically actuated soft robots have promising capabilities such as inherent compliance and user safety. The control of soft robots needs to properly handle nonlinear actuation dynamics, motion constraints, workspace limitations, and variable shape stiffness, so having a unique algorithm for all these issues would be extremely beneficial. In this work, we adapt Model Predictive Control (MPC), popular for rigid robots, to a soft robotic arm called SoPrA. We address the challenges that current control methods are facing, by proposing a framework that handles these in a modular manner. While previous work focused on Joint-Space formulations, we show through simulation and experimental results that Task-Space MPC can be successfully implemented for dynamic soft robotic control. We provide a way to couple the Piece-wise Constant Curvature and Augmented Rigid Body Model assumptions with internal and external constraints and actuation dynamics, delivering an algorithm that unites these aspects and optimizes over them. We believe that a MPC implementation based on our approach could be the way to address most of model-based soft robotics control issues within a unified and modular framework, while allowing to include improvements that usually belong to other control domains such as machine learning techniques.

### Model-Based Disturbance Estimation for a Fiber-Reinforced Soft Manipulator Using Orientation Sensing
Wednesday 11:10-11:20, Paper WeA-5.8
{: .notice}

**Authors:** Cangan, Barnabas Gavin	and Zhang, Yu and Katzschmann, Robert Kevin(ETH Zürich); Escaida Navarro, Stefan	and Duriez, Christian (Inria); Bai, Yang	(TU Berlin)

**Abstract:** A soft robotic arm should ideally be working efficiently, robustly, and safely in human-centered environments to provide assistance in real-world situations. For this goal, soft robots need to be able to estimate their state and external interactions based on (proprioceptive) sensors. Estimating disturbances allows a soft robot to perform desirable force control. Even in the case of rigid manipulators, force estimation at the end-effector is seen as a non-trivial problem. And indeed, other current approaches to address this challenge have shortcomings that prevent their general application. They are often based on simplified soft dynamic models, such as the ones relying on a piece-wise constant curvature approximation or matched rigid-body models that do not represent enough details of the problem. Thus, the applications needed for complex human-robot interaction can not be built. Finite element method (FEM) based modelings allow for predictions of soft robot dynamics in a more generic fashion. Here, using the soft robot modeling capabilities of the framework SOFA, we build a detailed FEM model of a multi-segment soft continuum robotic arm composed of compliant deformable materials and fiber-reinforced pressurized actuation chambers. In addition, a model for sensors that provide orientation output is presented. This model is used to establish a state observer for the manipulator. The sensor model is adequate for representing the output of flexible bend sensors as well as orientations provided by IMUs or coming from tracking systems, all of which are popular choices in soft robotics. Model parameters were calibrated to match imperfections of the manual fabrication process using physical experiments. We then solve a quadratic programming inverse dynamics problem to compute the components of external force that explain the pose error. Our experiments show an average force estimation error of around 1.2%. As the methods proposed are generic, these results are encouraging for the task of building soft robots exhibiting complex, reactive, sensor-based behavior that can be deployed in human-centered environments.

### Task-Space Control of Continuum Robots Using Underactuated Discrete Rod Models
Wednesday 14:40-14:50, Paper WeB-5.1
{: .notice}

**Authors:** Rucker, Caleb and Gaston, Joshua	(University of Tennessee); Barth, Eric J.	and Gallentine, James(Vanderbilt University)

**Abstract:** Underactuation is a core challenge associated with controlling soft and continuum robots, which possess theoretically infinite degrees of freedom, but few actuators. However, m actuators may still be used to control a dynamic soft robot in an m-dimensional output task space. In this paper we develop a task-space control approach for planar continuum robots that is robust to modeling error and requires very little sensor information. The controller is based on a highly underactuated discrete rod mechanics model in maximal coordinates and does not require conversion to a classical robot dynamics model form. This promotes straightforward control design, implementation and efficiency. We perform input-output feedback linearization on this model, apply sliding mode control to increase robustness, and formulate an observer to estimate the full state from sparse output measurements. Simulation results show exact task-space reference tracking behavior can be achieved even in the presence of significant modeling error, inaccurate initial conditions, and output-only sensing.

### Geometrically-Exact Inverse Kinematic Control of Sof Manipulators with General Threadlike Actuators’ Routing
Wednesday 15:10-15:20, Paper WeB-5.4
{: .notice}

**Authors:** Renda, Federico and Armanini, Costanza	and Mathew, Anup Teejo	(Khalifa University); Boyer, Frédéric	(Ecole Des Mines De Nantes)

**Abstract:** The inverse kinematic control of soft robots appears as an open challenge that has been the subject of a number of papers presented in the last decade. Some solutions have been provided based on specific assumptions on the robot’s shape or the actuation mechanism. Other more generic approaches are characterized by a significant computational cost or by a low level of accuracy for very high deformations. In the effort to overcome some of these limitations, here we present a Geometrically-Exact (GE) inverse kinematics controller, which can be applied to soft manipulators having general threadlike actuators’ routing. Being GE, the approach is suitable to applications involving arbitrarily large bending and twisting, and, on the other side, it relies on a reduced number of Degrees of Freedom (DOFs). We prove the feasibility of the proposed Jacobian-based inverse kinematic control in simulation for soft manipulators with complex and discontinuous actuators’ routing.


### Hybrid Eye-In-Hand/Eye-To-Hand Image Based Visual Servoing for Soft Continuum Arms
Wednesday 17:20-17:30, Paper WeC-5.7
{: .notice}

**Authors:** AlBeladi, Ali (King Fahd University of Petroleum & Minerals); Ripperger, Evan and Krishnan, Girish(University of Illinois  Urbana Champaign); Hutchinson, Seth	(Georgia Institute of Technology)

**Abstract:** Soft continuum arms (SCAs) that are controlled by visual servoing (VS) present trade-offs between the camera range and tracking accuracy. Cameras placed at a distance (eye-to-hand) can observe a larger workspace area and the SCA tip, while a camera at the end effector (eye-in-hand) can more accurately survey the target. In this letter, we present a hybrid eye-to-hand and eye-in-hand VS scheme to track a desired object in the SCA's worksapce. When the target is not in the field-of-view of the tip camera, hand-to-eye VS is implemented using a wide field-of-view camera on the soft robot's base, to servo the soft robot's tip to a feasible region where the target is expected to be seen by the tip camera. This region is estimated by solving an optimization problem that finds the best region to place the SCA assuming a constant curvature model for the SCA. When the target is seen by the tip camera, the system switches to a hand-in-eye controller that keeps the target in the desired image position of the tip camera. Experimental results on the popular BR^2 SCA demonstrates the effectiveness of the hybrid VS scheme under practical settings that include external disturbances.

### Deep-Learning-Based Compliant Motion Control of a Pneumatically-Driven Robotic Catheter
Wednesday 11:00-11:10, Paper WeA-7.7
{: .notice}

**Authors:** Wu, Di	and Ha, Xuan Thao and Zhang, Yao and Borghesan, Gianni and Vander Poorten, Emmanuel B (KU Leuven); Ourak, Mouloud (University of Leuven); Niu, Kenan	(University of Twente); Trauzettel, Fabian and Dankelman, Jenny (TU Delft); Menciassi, Arianna (Scuola Superiore Sant'Anna)

**Abstract:** In cardiovascular interventions, when steering catheters and especially robotic catheters, great care should be paid to prevent applying too large forces on the vessel walls as this could dislodge calcifications, induce scars or even cause perforation. To address this challenge, this paper presents a novel compliant motion control algorithm that relies solely on position sensing of the catheter tip and knowledge of the catheter's behavior. The proposed algorithm features a data-driven tip position controller. The controller is trained based on a so-called control Long Short-Term Memory Network (control-LSTM). Trajectory following experiments on four different trajectories are conducted to validate the quality of the proposed control-LSTM. The performance was compared with the performance of a controller that makes use of an analytical hysteresis model, i.e. the inverse Deadband Rate-Dependent Prandtl-Ishlinskii (IDRDPI) model. Results demonstrated superior positioning capability with sub-degree precision of the new approach in the presence of severe rate-dependent hysteresis. Experiments both in a simplified setup as well as in an aortic phantom further show that the proposed approach allows reducing the interaction forces with the environment by around 70%. This work shows how deep learning can be exploited advantageously to avoid tedious modeling that would be needed to precisely steer continuum robots in constrained environments such as the patient's vasculature.
 