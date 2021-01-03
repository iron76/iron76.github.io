---
permalink: /research/
title: "Research"
excerpt: "Francesco's research topics."
layout: single
author_profile: true
last_modified_at: 2021-01-01T14:51:23-04:00
toc: true
---

## 2020 - 2018
At Deepmind I have been progressively more interested in reinforcement learning on real robots. I have  gained experience with the problems underling the application of deep neural networks at scale in the field of robotics. This new line of research have produced relevant publications in the area of:
* **learning from demonstrations**, i.e. learning using the prior knowledge embedded in a successful execution of the task;
* **sim-to-real transfer**, i.e. learning in augmented simulation and transferring on the real robot;
* **learning from scratch**, i.e. learning primarily with real-robot data and minimising prior knowledge.

### Learning real-world tasks from demonstrations
<em> with R. Jeong, F. Romano, J. Kay, D. Khosid, and K. Bousmalis </em>

#### Learning Dexterous Manipulation from Suboptimal Experts

<iframe width="560" height="315" src="https://youtube.com/embed/qTZ1oh6KVoc" frameborder="0" allowfullscreen></iframe>

<p> In this research investigation, we introduce Relative Entropy Q-Learning (REQ), a simple policy iteration algorithm that combines ideas from successful offline and conventional RL algorithms. It represents the optimal policy via importance sampling from a learned prior and is well-suited to take advantage of mixed data distributions.  We demonstrate experimentally that REQ outperforms several strong baselines on robotic manipulation tasks for which sub-optimal experts are available. We show how suboptimal experts can be constructed effectively by composing simple waypoint tracking controllers, and we also show how learned primitives can be combined with waypoint controllers to obtain reference behaviours to bootstrap a complex manipulation task on a simulated bimanual robot with human-like hands.</p>

<h4>References</h4>
<li> Jeong, Rae, et al. "Learning Dexterous Manipulation from Suboptimal Experts." arXiv preprint arXiv:2010.08587 (2020).</li>

### Learning real-world tasks from simulations
<em> with R. Jeong, F. Romano, J. Kay, D. Khosid, and K. Bousmalis </em>

#### Self-Supervised Sim-to-Real Adaptation for Visual Robotic Manipulation

<iframe width="560" height="315" src="https://youtube.com/embed/pmLASU_MW_o" frameborder="0" allowfullscreen></iframe>

<p> In this work, we learn a latent state representation implicitly with deep reinforcement learning in simulation, and then adapt it to the real domain using unlabelled real robot data. We propose to do so by optimising sequence-based self-supervised objectives. These exploit the temporal nature of robot experience, and can be common in both the simulated and real domains, without assuming any alignment of underlying states in simulated and unlabelled real images. We propose Contrastive Forward Dynamics loss, which combines dynamics model learning with time-contrastive techniques.</p>

#### Modelling Generalized Forces with Reinforcement Learning for Sim-to-Real Transfer

<iframe width="560" height="315" src="https://youtube.com/embed/2diszIMOn6A" frameborder="0" allowfullscreen></iframe>

<p> In this work, We use reinforcement learning to efficiently optimise the mapping from states to generalised forces over a discounted infinite horizon. We show that using only minutes of real world data improves the sim-to-real control policy transfer. We demonstrate the feasibility of our approach by validating it on a non-prehensile manipulation task on the Sawyer robot.</p>


<h4>References</h4>
<li> Jeong, Rae, et al. "Self-supervised sim-to-real adaptation for visual robotic manipulation." 2020 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2020.</li>
<li> Jeong, Rae, et al. "Modelling Generalized Forces with Reinforcement Learning for Sim-to-Real Transfer." arXiv preprint arXiv:1910.09471 (2019).</li>

### Learning real-world tasks with minimal prior
<em> with M. Martins, G. Vezzani, T. Lampe, M. Neunert, M. Riedmiller </em>

#### Ball-in-a-cup

<iframe width="560" height="315" src="https://youtube.com/embed/AX6rK2xywng" frameborder="0" allowfullscreen></iframe>

<p> This research activity presents a method for fast training of vision based control policies on real robots. The key idea behind our method is to perform multi-task Reinforcement Learning with auxiliary tasks that differ not only in the reward to be optimised but also in the state-space in which they operate. In particular, we allow auxiliary task policies to utilise task features that are available only at training-time. This allows for fast learning of auxiliary policies, which subsequently generate good data for training the main, vision-based control policies. </p>

#### Peg-in-hole

<iframe width="560" height="315" src="https://youtube.com/embed/JnvdNpWAia4" frameborder="0" allowfullscreen></iframe>

<p> We propose a challenging, highly under-actuated peg-in-hole task with a free, rotational asymmetrical peg, requiring a broad range of manipulation skills. While correct peg (re-)orientation is a requirement for successful insertion, there is no reward associated with it. Hence an agent needs to understand this pre-condition and learn the skill to fulfill it. The final insertion reward is sparse, allowing freedom in the solution and leading to complex emerging behaviour not envisioned during the task design.  </p>

<h4>References</h4>
<li> Schwab, Devin, et al. "Simultaneously learning vision and feature-based control policies for real-world ball-in-a-cup." arXiv preprint arXiv:1902.04706 (2019).</li>
<li> Vezzani, Giulia, et al. ""What, not how"--Solving an under-actuated insertion task from scratch." arXiv preprint arXiv:2010.15492 (2020).</li>


## 2018

<p> Before joining Deepmind, I have been involved in several European projects. Here is a list of the most relevant projects for which I am involved as a scientific responsible (i.e. principal investigator). Below follow a summary of the the research projects I have been involved in. For a complete list of papers see my publications list.</p>

<li><a href="http://www.andy-project.eu/">H2020 AnDy </a>(coordinator)</li>
<li><a href="http://www.codyco.eu/">FP7 CoDyCo </a>(coordinator)</li>
<li><a href="http://orb.iwr.uni-heidelberg.de/koroibot/">FP7 Koroibot </a>(principal investigator)</li>

### Whole-body dynamics with contact switching
<em> with D. Pucci, F. Romano, G. Nava, S. Traversaro, S. Dafarra and F. Andrade </em>

<iframe width="560" height="315" src="https://youtube.com/embed/9XRI4BeXN78" frameborder="0" allowfullscreen></iframe>

<p> This research activity concerns the control of the iCub whole-body posture in situations which involve breaking and establishing contacts. At present, this research benefits of recent results in force/torques sensor calibration, proof of stability of inverse dynamic control approaches. </p>

<p>
 <strong>Open-source software repository</strong>: 
(1) <a href="https://github.com/S-Dafarra/WBI-Toolbox-controllers">WBI-Toolbox-controllers for step recovery</a>,
(2) <a href="https://github.com/robotology/codyco-modules">codyco-modules</a>,
(3) <a href="https://github.com/robotology-playground/WBI-Toolbox">WBI-Toolbox</a>. 
</p>

<h4>References</h4>
<li>Dafarra S., Romano F. & Nori F. 2016, ‘Torque-Controlled Stepping-Strategy Push Recovery: Design and Implementation on the iCub Humanoid Robot’, IEEE-RAS International Conference on Humanoid Robots, Cancun, Mexico,November 15-17 2016. </li>
<li> Pucci D., Nava G. & Nori F. 2016, ‘An Automatic Gain Tuning Method of a Momentum Based Balancing Controller for Humanoid Robots’, IEEE/RAS International Conference of Humanoids Robots, Cancun, Mexico,November 15-17 2016.</li>
<li> Nuno Guedelha, Naveen Kuppuswamy, Silvio Traversaro & Francesco Nori 2016, ‘Self-calibration of Joint Offsets for Humanoid Robots Using Accelerometer Measurements’, 2016 IEEE-RAS International Conference on Humanoid Robots.</li>

### Whole-Body Dynamics Control
<em> with D. Pucci, F. Romano and G. Nava  </em>

<iframe width="560" height="315" src="https://www.youtube.com/embed/VrPBSSQEr3A" frameborder="0" allowfullscreen></iframe>

<p> This research activity concerns the control of the iCub whole-body posture exploiting whole-body distributed contacts. This research activity is based on the iCub ability to control joint torques and to detect external contacts through whole-body distributed tactile sensors (i.e. artificial skin). </p>

<p> 
 <strong>Open-source software repository</strong>: 
 (1) <a href="https://github.com/robotology-playground/WBI-Toolbox-controllers">WBI-Toolbox-controllers</a>,
 (2) <a href="https://github.com/robotology/codyco-modules">codyco-modules</a>,
 (3) <a href="https://github.com/robotology-playground/WBI-Toolbox">WBI-Toolbox</a>. 
</p>

<h4>References</h4>
<li> Nori F., Traversaro S., Eljaik J., Romano F., Del Prete A. & Pucci D. 2015, ‘iCub whole-body control through force regulation on rigid non-coplanar contacts’, Frontiers in Robotics and AI. </li>
<li> Pucci D., Romano F. & Nori F. 2015, ‘Collocated Adaptive Control of Underactuated Mechanical Systems’, IEEE Transactions on Robotics. </li>

### Whole-Body Dynamics Modeling and Identification
<em> with S. Traversaro, R. Camoriano </em>

<iframe width="560" height="315" src="https://www.youtube.com/embed/UXU3KSa201o" frameborder="0" allowfullscreen></iframe>
<p> This research activity concerns the problem of modeling the whole-body  dynamics of an articulated rigid-body structure. Focus is on computational efficiency which is obtained by implementing state-of-the-art inverse and forward dynamics algorithms (Featherstone 2007). This research activity includes the iCub simulations which include available (e.g. Gazebo) and custom (e.g. mex-wholebodymodel) open-source software </p>

<p> 
 <strong>Open-source software repository</strong>: 
 (1) <a href="https://github.com/robotology/mex-wholebodymodel">mex-wholebodymodel</a>,
 (2) <a href="https://github.com/robotology/gazebo-yarp-plugins">gazebo-yarp-plugins</a>,
</p>

<h4>References</h4>
<li> Mingo H.E., Traversaro S., Alessio R., Mirko F., Settimi A., Romano F., Natale L., Bicchi A., Nori F. & Tsagarakis G. Nikos 2014, ‘A YARP based plugin for Gazebo Simulator’, 2014 Modelling and Simulation for Autonomous Systems, Rome, Italy, 5-6, May, 2014. </li>


### Whole-Body Dynamics Estimation 
<em> with S. Traversaro, M. Fumagalli and S. Ivaldi </em>

<iframe width="560" height="315" src="https://www.youtube.com/embed/yQGXYGS0Ojo" frameborder="0" allowfullscreen></iframe>

<p> This research activity concerns the estimation of dynamic quantities (e.g. joint torques, joint accelerations, joint velocities, external forces) from whole-body distributed heterogenous sensors (e.g. artificial skin, accelerometers, gyroscopes, force/torque sensors). </p>

<p> 
 <strong>Open-source software repository</strong>: 
 (1) <a href="https://github.com/iron76/bnt_time_varying">bnt_time_varying</a>,
 (2) <a href="https://github.com/robotology/idyntree">idyntree</a>,
 (3) <a href="http://wiki.icub.org/brain/idyn_introduction.html">idyn</a>. 
</p>

<h4>References</h4>
<li> Nori F., Kuppuswamy N. & Traversaro S. 2015, ‘Simultaneous state and dynamics estimation in articulated structures’, IEEE/RSJ International Conference on Intelligent Robots and Systems (2015), Hamburg, Germany, October (29 September - 1 October, 2015). </li>
<li> S. Traversaro, A. Del Prete, S. Ivaldi, and F. Nori. Inertial parameters identification and joint torques estimation with proximal force/torque sensing. In Robotics and Automation (ICRA), 2015 IEEE Inter- national Conference on, pages 2105–2110. IEEE, 2015. </li>
<li> Ciliberto C., Fiorio L., Maggiali M., Natale L.R. L., Metta G., Sandini G. & Nori F. 2014, ‘Exploiting global force torque measurements for local compliance estimation in tactile arrays’, IEEE/RSJ International Conference on Intelligent Robots and Systems, Chicago, Illinois, September 14-18, 2014. </li>
<li> Fumagalli M., Ivaldi S., Randazzo M., Natale L., Metta G., Sandini G. & Nori F. 2012, ‘Force feedback exploiting tactile and proximal force/torque sensing. Theory and implementation on the humanoid robot iCub.’, Autonomous Robots, vol. 33,no. 4, pp. 381–398. </li>	
