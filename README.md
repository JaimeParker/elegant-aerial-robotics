<h1 align="center">空中机器人的技艺 Elegant-Aerial-Robotics</h1>

# Content 目录

<nav>
    <ul>
        <li><a href="#introduction">1. Introduction</a></li>
        <li><a href="#generalized-aerial-robots">2. Generalized Aerial Robots 广义空中机器人</a>
            <ul>
                <li><a href="#multicopter">2.1 Multicopter 多旋翼</a>
                    <ul>
                        <li><a href="#mc-configuration">2.1.1 Multicopter-Configuration 按构型</a></li>
                        <li><a href="#mc-media">2.1.2 Multicopter-Media 按介质</a></li>
                        <li><a href="#mc-modal">2.1.3 Multicopter-Modal 按模态</a></li>
                        <li><a href="#mc-actuate">2.1.4 Multicopter-Actuate 按驱动</a></li>
                        <li><a href="#mc-jointlink">2.1.5 Multicopter-Link 按挂载</a></li>
                    </ul>
                </li>
                <li><a href="#vtol">2.2 (E)VTOL 垂起固定翼</a></li>
                <li><a href="#fixed-wing">2.3 Fixed-Wing 固定翼</a></li>
                <li><a href="#helicopter">2.4 Helicopter 直升机</a></li>
                <li><a href="#balloon">2.5 Balloon 气球/飞艇</a></li>
                <li><a href="#ornithopter">2.6 Ornithopter 扑翼机</a></li>
            </ul>
        </li>
        <li><a href="#research">3. Research 主要研究方向</a>
            <ul>
                <li><a href="#auto-flight">3.1 Autonomous Flight 自主飞行</a></li>
                <li><a href="#racing">3.2 Racing 竞速/大机动飞行</a></li>
                <li><a href="#flight-control">3.3 Flight Control 飞行控制</a></li>
                <li><a href="#exploration">3.4 Exploration 探索</a></li>
                <li><a href="#swarm">3.5 Swarm 集群</a></li>
                <li><a href="#state-estimation">3.6 State Estimation 状态估计</a></li>
                <li><a href="#aerial-manipulation">3.7 Aerial Manipulation 空中操作</a></li>
                <li><a href="#novel-design">3.8 Novel/Morphing Design 新构型设计/变形无人机</a></li>
            </ul>
        </li>
        <li><a href="#tech-stack">4. Tech stack 技术栈</a>
            <ul>
                <li><a href="#general-design">4.1 General Design 总体设计</a>
                    <ul>
                        <li><a href="#pure-self-design">4.1.1 Self-Design 自主设计</a></li>
                        <li><a href="#buy-as-need">4.1.2 Buy-as-Needed 采购</a></li>
                    </ul>
                </li>
                <li><a href="#dynamics">4.2 Dynamics 动力学</a>
                    <ul>
                        <li><a href="#fluid mechanics">4.2.1 Fluid Mechanics流体力学</a></li>
                        <li><a href="#aerodynamics">4.2.2 Aerodynamics空气动力学</a></li>
                        <li><a href="#flightdynamics">4.2.3 Flight Dynamics飞行力学</a></li>
                    </ul>
                </li>
                <li><a href="#mechanics">4.3 Mechanics 机械</a></li>
                <li><a href="#embedded">4.4 Embedded 嵌入式</a>
                    <ul>
                        <li><a href="#stm32">4.4.1 STM32</a></li>
                        <li><a href="#nuttx">4.4.2 NuttX</a></li>
                        <li><a href="#Pixhawk">4.4.3 Pixhawk</a></li>
                        <li><a href="#other-flight-hardware">4.4.4 Other Flight Hardware</a></li>
                    </ul>
                </li>
                <li><a href="#communication">4.5 Communication 通信</a>
                    <ul>
                        <li><a href="#communication-basis">4.5.1 Communication Basics 通信原理</a></li>
                        <li><a href="#uart">4.5.2 UART</a></li>
                        <li><a href="#CAN">4.5.3 CAN</a></li>
                        <li><a href="#ROS">4.5.4 ROS及功能包</a></li>
                    </ul>
                </li>
                <li><a href="#sensing">4.6 Sensing/Perception 传感/感知</a>
                    <ul>
                        <li><a href="#sensors">4.6.1 Sensors 传感器</a></li>
                        <li><a href="#sensing/state-estimation">4.6.2 State Estimation 状态估计</a></li>
                        <li><a href="#tracking">4.6.3 Tracking 目标跟踪</a></li>
                    </ul>
                </li>
                <li><a href="#control">4.7 Control 控制</a>
                    <ul>
                        <li><a href="#control-basis">4.7.1 Control Basics 控制原理</a></li>
                        <li><a href="#control-methods">4.7.2 Control Methods 控制方法</a></li>
                        <li><a href="#control-architecture">4.7.3 PX4-Autopilot PX4飞控</a></li>
                        <li><a href="#optimal-control-optimization">4.7.4 Optimal Control and Optimization 最优控制与优化</a></li>
                    </ul>
                </li>
                <li><a href="#planning">4.8 Planning 规划</a>
                    <ul>
                        <li><a href="#path-planning">4.8.1 Path Planning 路径规划</a></li>
                        <li><a href="#trajectory-planning">4.8.2 Trajectory Planning 轨迹规划</a></li>
                        <li><a href="#motion-planning">4.8.3 Motion Planning 运动规划</a></li>
                        <li><a href="#task-planning">4.8.4 Task Planning 任务规划</a></li>
                    </ul>
                </li>
                <li><a href="#simulation">4.9 Simulation 仿真</a>
                    <ul>
                        <li><a href="#gazebo">4.9.1 Gazebo</a></li>
                        <li><a href="#air-sim">4.9.2 AirSim</a></li>
                        <li><a href="#Flightmare">4.9.3 Flightmare</a></li>
                        <li><a href="#Rotors-simulation">4.9.4 Rotors Simulation</a></li>
                        <li><a href="#Issac-Sim">4.9.5 Issac Sim</a></li>
                        <li><a href="#Aerial-Gym">4.9.6 Aerial Gym</a></li>
                    </ul>
                </li>
                <li><a href="#real-flight">4.10 Real Flight 实机</a>
                    <ul>
                        <li><a href="#remote-control">4.10.1 Remote Control 遥控</a></li>
                        <li><a href="#QGC">4.10.2 QGC</a></li>
                        <li><a href="#flight-log">4.10.3 Flight Log 飞行日志</a></li>
                        <li><a href="#companion-computer">4.10.4 Companion Computer 上位机</a></li>
                    </ul>
                </li>
                <li><a href="#nn-methods">4.11 NN Methods learning方法</a>
                    <ul>
                        <li><a href="#reinforcement-learning">4.11.1 Reinforcement Learning 强化学习</a></li>
                        <li><a href="#generative-models">4.11.2 Generative Models 生成模型</a></li>
                        <li><a href="#LLM">4.11.3 (M)LLMs （视觉等模态）大语言模型</a></li>
                    </ul>
                </li>
            </ul>
        </li>
        <li><a href="#labs-home">5. Labs and Homepages</a>
            <ul>
                <li><a href="#domestic">5.1 Domestic(PRC) 国内</a>
                    <ul>
                        <li><a href="#chinamainland">5.1.1 Mainland PRC 中国大陆</a></li>
                        <li><a href="#hongkong">5.1.2 Hongkong, China 中国香港</a></li>
                    </ul>
                </li>
                <li><a href="#overseas">5.2 Overseas(Out of PRC) 国外</a>
                    <ul>
                        <li><a href="#north-america">5.2.1 North America 北美</a></li>
                        <li><a href="#europe">5.2.2 Europe 欧洲</a></li>
                        <li><a href="#asia">5.2.3 Asia 亚洲</a></li>
                    </ul>
                </li>
            </ul>
        </li>
    </ul>
</nav>

<section id="introduction"></section>

# 1. Introduction

空中机器人是一类具有飞行能力的机器人，其学习与研究涉及到多个学科，因此从0到1的学习曲线较长。

为了方便大家学习与研究空中机器人，我们整理了一个空中机器人学习的知识体系，欢迎大家补充与交流。

**为什么要构建这样的大纲**（每部分的作用）：

* **Generalized Aerial Robots 广义空中机器人** 部分主要介绍空中机器人的构型与分类，做一个科普和初步了解
* **Research 研究方向** 部分主要放一些新工作和经典文章
* **Tech Stack 技术栈** 部分主要放一些相关的技术与工具，介绍**学习路线**和好用的小工具，repo等

**如何贡献(非repo协作者)**:

* fork本项目，创建你自己的分支branch
* 在你的分支上进行修改，别忘了把贡献及你想留下的信息放到[Contributors](Contributors.md)中
* add, commit, push
* 创建一个pull request到主分支

对于repo的协作者，**欢迎直接在主分支上进行修改**。

<section id="generalized-aerial-robots"></section>

# 2. Generalized Aerial Robots 广义空中机器人

从构型出发，我们首先从空中机器人本体进行介绍。

<img src="./assets/images/广义空中机器人generalized aerial robots.png" alt="Generalized Aerial Robots" width="600px"/>

<section id="multicopter"></section>

## 2.1 Multicopter 多旋翼

这里会对多旋翼进行一个简单介绍，所以不会罗列详细的工作，更接近于科普。

多旋翼是空中机器人中最常见的类型，通常由多个旋翼组成。
以下会介绍多旋翼的几种分类方式，做到尽可能地独立，但仍然无法避免交叉。

<section id="mc-configuration"></section>

### 2.1.1 Multicopter-Configuration 按构型

这里准确想表达的是变形的能力(morphing/deformable)，虽然以多旋翼为基础的空中机器人构型各式各样，但可以将其分为能够变形和不能变形两大类。

列举几个工作（若作为科普，可以直接看YouTube）：
* [Design, Modeling, and Control of an Aerial Robot DRAGON: A Dual-Rotor-Embedded Multilink Robot With the Ability of Multi-Degree-of-Freedom Aerial Transformation](https://ieeexplore.ieee.org/document/8258850)，[[YouTube]](https://www.youtube.com/watch?v=ZDYU22qNI_Q)，ICRA 2018，Dragon Lab，多关节可变形一家独大
* [Design and Control of a Passively Morphing Quadcopter](https://ieeexplore.ieee.org/document/8794373), [[YouTube]](https://www.youtube.com/watch?v=MSvoQT__c9U)，ICRA 2019，HiPeRLab，可变形四旋翼
* [Biomimetic Morphing Quadrotor Inspired by Eagle Claw for Dynamic Grasping](https://ieeexplore.ieee.org/document/10495172), TRO 2024，IRMV Lab，仿生变形四旋翼
* [Ring-Rotor: A Novel Retractable Ring-Shaped Quadrotor With Aerial Grasping and Transportation Capability](https://ieeexplore.ieee.org/document/10044964), [[bilibili]](https://www.bilibili.com/video/BV1gY4y1K723), Fast Lab ZJU, “伸缩”四旋翼；后续的工作Shape-Adaptive Planning and Control for a Deformable Quadrotor，[[bilibili]](https://www.bilibili.com/video/BV14eRpYnE8K/)，submitted to IROS 2025，Fast Lab ZJU，变形四旋翼的规划
* [The Foldable Drone: A Morphing Quadrotor That Can Squeeze and Fly](https://ieeexplore.ieee.org/document/8567932), RAL 2018, RPG UZH

另外bi-copter的工作：
* [Gemini II: Design, Modeling, and Control of a Compact Yet Efficient Servoless Bi-copter](https://ieeexplore.ieee.org/document/9736334), [[YouTube]](https://www.youtube.com/watch?v=qGhQbPtp7Sw&t=2s), TMECH 2022, MaRS Lab HKU


<section id="mc-media"></section>

### 2.1.2 Multicopter-Media 按介质

多见于跨空气-水-地面（结合）介质的空中机器人。

* [Toward a gliding hybrid aerial underwater vehicle: Design, fabrication, and experiments](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.22063), JFR 2022, SJTU，“哪吒III（垂起固定翼式）”海空跨域无人航行器

<section id="mc-modal"></section>

### 2.1.3 Multicopter-Modal 按模态

* [Miniature deep-sea morphable robot with multimodal locomotion](https://www.science.org/doi/10.1126/scirobotics.adp7821), Science Robotics 2025, BUAA, [文力](http://www.me.buaa.edu.cn/info/1071/2298.htm)，[丁希仑](http://www.me.buaa.edu.cn/info/1071/2141.htm)，虽然是水下多模态，但太大佬了
* [Design, Modeling, and Control of a Quadruped Robot SPIDAR: Spherically Vectorable and Distributed Rotors Assisted Air-Ground Quadruped Robot](https://ieeexplore.ieee.org/document/10113721), [[YouTube]](https://www.youtube.com/watch?v=lLvsxmJUyCk), RAL 2023, Dragon Lab，飞行与爬行模态，Multi-Modal Locomotion也是他们的研究方向之一
* [Skater: A Novel Bi-Modal Bi-Copter Robot for Adaptive Locomotion in Air and Diverse Terrain](https://ieeexplore.ieee.org/document/10538378), [[bilibili]](https://www.bilibili.com/video/BV1y2421M7HM/), RAL 2024, Fast Lab ZJU，飞行与滚动模态；以及之前的[Model-Based Planning and Control for Terrestrial-Aerial Bimodal Vehicles with Passive Wheels](https://ieeexplore.ieee.org/document/10342188), [[bilibili]](https://www.bilibili.com/video/BV1Dj411M7Uh)
* [DoubleBee: A Hybrid Aerial-Ground Robot with Two Active Wheels](https://ieeexplore.ieee.org/document/10341984), IROS 2023, AirLab CMU

<section id="mc-actuate"></section>

### 2.1.4 Multicopter-Actuate 按驱动

以四旋翼无人机举例，传统的构型是欠驱动的，即只有四个控制输入（四个电机），而有六个自由度（x、y、z、roll、pitch、yaw）。

全驱动则可以通过改变电机位姿或其他方法来实现。

* [Fully Actuated Multirotor UAVs: A Literature Review](https://ieeexplore.ieee.org/document/8978486?arnumber=8978486), RAM 2020
* [The Voliro Omniorientational Hexacopter: An Agile and Maneuverable Tiltable-Rotor Aerial Vehicle](https://ieeexplore.ieee.org/document/8485627/), RAM 2018
* [FLOAT Drone: A Fully-actuated Coaxial Aerial Robot for Close-Proximity Operations](https://arxiv.org/abs/2503.00785) [[Website]](https://zju-jxlin.github.io/float-drone.github.io/), [[bilibili]](https://www.bilibili.com/video/BV1svRpYSE9c/) submitted to IROS 2025, Fast Lab ZJU, 解决气流反作用力

<section id="mc-jointlink"></section>

### 2.1.5 Multicopter-Link 按挂载

多旋翼+刚体/灵巧/软体臂的方案就很多了，以下列举一些：

* [Past, Present, and Future of Aerial Robotic Manipulators](https://ieeexplore.ieee.org/document/9462539), TRO 2022, Antonio Franchi
* [AeCoM: An Aerial Continuum Manipulator With  IMU-Based Kinematic Modeling and  Tendon-Slacking Prevention](https://ieeexplore.ieee.org/document/10081306), TSMC 2023, ArcLab HKU, 灵巧臂
* [A dexterous and compliant aerial continuum manipulator for cluttered and constrained environments](https://www.nature.com/articles/s41467-024-55157-2), Nature 2025, ArcLab 2025, 灵巧臂“会飞的象鼻”
* [A Compact Aerial Manipulator: Design and Control for Dexterous Operations](https://link.springer.com/article/10.1007/s10846-024-02090-7), JIRS 2024, BUAA 郭雷组, [Liu_Qianyuan [bilibili]](https://space.bilibili.com/21343190)，[Zeshuai Chen](https://scholar.google.com.hk/citations?user=p9G9KU8AAAAJ&hl=zh-CN&oi=ao)，自研飞控，manipulator设计，抗扰控制，灵巧操作
* [Millimeter-Level Pick and Peg-in-Hole Task Achieved by Aerial Manipulator](https://ieeexplore.ieee.org/abstract/document/10339889), TRO 2023, BUAA 郭雷组


<section id="vtol"></section>

## 2.2 (E)VTOL 垂起固定翼

<section id="fixed-wing"></section>

## 2.3 Fixed-Wing 固定翼

<section id="helicopter"></section>

## 2.4 Helicopter 直升机

<section id="balloon"></section>

## 2.5 Balloon 气球/飞艇

<section id="ornithopter"></section>

## 2.6 Ornithopter 扑翼机



<section id="research"></section>

# 3. Research 主要研究方向与最新研究

<img src="./assets/images/研究方向Aerial Robotics Research.png" alt="Aerial Robotics Research" width="600px"/>

<section id="auto-flight"></section>

## 3.1 Autonomous Flight 自主飞行

自主飞行包含感知，规划与控制等方面的工作。如果粗糙地将其分类，可以分成基于优化的和基于学习的两大类。其中，基于优化的往往采用前端+后端的方法，而基于学习的则各式各样。

近期的工作：
* [Safety-assured high-speed navigation for MAVs](https://www.science.org/doi/10.1126/scirobotics.ado6187), Science Robotics 2025, MaRS Lab HKU
* [Flying on Point Clouds with Reinforcement Learning](http://arxiv.org/abs/2503.00496), ArXiv 2025, Fast Lab ZJU, 对PCL做处理用RL
* [MAVRL: Learn to Fly in Cluttered Environments With Varying Speed](https://ieeexplore.ieee.org/document/10816139), MAVLab 2025 TUDelft, varying speed（以致扩展到accel等参数）是一个很重要的点，记得高飞老师也有几篇类似的工作
* [Flying in Highly Dynamic Environments With  End-to-End Learning Approach](https://ieeexplore.ieee.org/abstract/document/10908845), RAL 2025, ArcLab HKU, 基于RL，可动态场景
* [RESC: A Reinforcement Learning Based Search-to-Control Framework for Quadrotor Local Planning in Dense Environments](https://arxiv.org/abs/2408.00275), [[code]](https://github.com/JaimeParker/resc-pilot), SJTU, 基于RL的局部规划器，对ESDF做处理提取低维obstacle info
* [Seeing Through Pixel Motion: Learning Obstacle Avoidance from  Optical Flow with One Camera](http://arxiv.org/abs/2411.04413), RAL 2025, SJTU, differential的idea，dual optical flow作为输入
* [NavRL: Learning Safe Flight in Dynamic Environments](https://ieeexplore.ieee.org/document/10904341), [[code]](https://github.com/Zhefan-Xu/NavRL), [[video]](https://www.bilibili.com/video/BV1gsA9eTErz), RAL 2025, CMU，基于强化学习的自主飞行，控到速度，基于Issac Sim
* [You Only Plan Once: A Learning-Based One-Stage Planner With Guidance Learning](https://ieeexplore.ieee.org/document/10528860/), [[code]](https://github.com/TJU-Aerial-Robotics/YOPO), [[video]](https://www.bilibili.com/video/BV15M4m1d7j5/), RAL 2024, TJU

基于优化的工作：
* [Minimum snap trajectory generation and control for quadrotors](https://ieeexplore.ieee.org/document/5980409), ICRA 2011, [Vijay Kumar](https://www.kumarrobotics.org/), UPenn，最早的轨迹规划工作之一，开山之作，提出四旋翼的微分平坦特性，可以用 x,y,z,yaw 及其导数来推导出12个量，因此轨迹多以x,y,z,yaw为主。
* [Continuous-time trajectory optimization for online UAV replanning](https://ieeexplore.ieee.org/document/7759784), IROS 2016, ASL ETH，提出了基于梯度的轨迹规划方法，后续的工作也都在这个基础上进行改进。
* 可以选择性地跳过一些基于gradient和Safe Flight Corridor的工作，直接看第一个标准优雅的规划器Fast-Planner的第一版，[Robust and Efficient Quadrotor Trajectory Generation for Fast Autonomous Flight](https://ieeexplore.ieee.org/document/8758904/), RAL 2019, HKUST Aerial Robotics Group；之后又有了第二、三版文章，分别聚焦于topological planning和perception-aware，[Robust Real-time UAV Replanning Using Guided Gradient-based Optimization and Topological Paths](https://ieeexplore.ieee.org/document/9196996/), ICRA 2020; [RAPTOR: Robust and Perception-Aware Trajectory Replanning for Quadrotor Fast Flight](https://ieeexplore.ieee.org/document/9422918/), TRO 2021
* ESDF free的[EGO-Planner: An ESDF-Free Gradient-Based Local Planner for Quadrotors](https://ieeexplore.ieee.org/document/9309347/), RAL 2021
* 最后到时空联合规划[[minco]](https://github.com/ZJU-FAST-Lab/GCOPTER), [Geometrically Constrained Trajectory Optimization for Multicopters](https://ieeexplore.ieee.org/document/9765821), TRO 2022, Fast Lab ZJU，提出了基于几何约束的轨迹优化方法，解决了多旋翼的时空联合规划问题。

<section id="racing"></section>

## 3.2 Racing 竞速/大机动飞行

我了解到的主要是 Prof. [Davide](https://rpg.ifi.uzh.ch/people_scaramuzza.html) 和 [高飞](http://zju-fast.com/research-group/fei-gao/)老师的工作：

Davide 的 Agile flight 和 Racing 有点交叉，主要基于优化，RL及differential做：

* [rpg research: Agile Drone Flight](https://rpg.ifi.uzh.ch/aggressive_flight.html) and [rpg research: Drone Racing](https://rpg.ifi.uzh.ch/research_drone_racing.html)，可以直接关注他们的research发布页，也可以关注 [publicaitons](https://rpg.ifi.uzh.ch/publications.html) 和 [Davide 的 Google Scholar](https://scholar.google.com/citations?user=SC9wV2kAAAAJ&hl=en)。
* [Environment as Policy: Learning to Race in Unseen Tracks](https://rpg.ifi.uzh.ch/env_as_policy/), ICRA 2025, one single racing policy efficiently learns to race in diverse and challenging tracks
* [Student-Informed Teacher Training](https://rpg.ifi.uzh.ch/sitt/), ICLR 2025 spotlight, 简称ST训练，与BC&DAgger对比，虽然在racing上没那么多实验涉及，但很有意思的工作
* [Dream to Fly: Model-Based Reinforcement Learning for Vision-Based Drone Flight](http://arxiv.org/abs/2501.14377), vision+RL
* 中间的一些工作这里不详细介绍了，直接看[rpg research: Agile Drone FLight](https://rpg.ifi.uzh.ch/aggressive_flight.html)，比如AC-MPC，MPCC++等，都是很好的工作，racinger们可以直接参考。
* [Autonomous Drone Racing: A Survey](https://ieeexplore.ieee.org/document/10530312), TRO 2024, racing survey
* [Reaching the limit in autonomous racing: Optimal control versus reinforcement learning](https://www.science.org/doi/10.1126/scirobotics.adg1462), Science Robotics 2023, 不知道有多少人是因为[Yunlong](https://yunlong-song.com/index.html)的这篇SR开始关注RL/learning与racing/agile flight的结合，这篇文章中论证的a better goal是很多面临“为什么要使用RL”时可以回答的一个问题。
* [Champion-level drone racing using deep reinforcement learning](https://www.nature.com/articles/s41586-023-06419-4)，以及这篇被广大公众号/自媒体转载的Nature文章
* [Learning Perception-Aware Agile Flight in Cluttered Environments](https://ieeexplore.ieee.org/abstract/document/10160563), 但其实 Yunlong 还做了很多其他的工作，在类似任务下，[Learning Minimum-Time Flight in Cluttered Environments](https://ieeexplore.ieee.org/document/9794627)
* [Learning High-Speed Flight in the Wild](https://rpg.ifi.uzh.ch/AgileAutonomy.html)

高飞老师则是model-based，到与learning结合：

* [Unlocking aerobatic potential of quadcopters: Autonomous freestyle flight generation and execution](https://www.science.org/doi/10.1126/scirobotics.adp9905), Science Robotics 2025, [[bilibili]](https://www.bilibili.com/video/BV1WXouYmEaW/)，先拿这篇SR镇楼，三年之作
* Automatic Generation of Aerobatic Flight in Complex Environments via Diffusion Models, [[bilibili]](https://www.bilibili.com/video/BV1sj5yznEmN/), 也开始diffusion了（diffusion policy+drone有很多做了的和在做的工作）
* [Fast-Racing: An Open-Source Strong Baseline for SE(3) Planning in Autonomous Drone Racing](https://ieeexplore.ieee.org/document/9543598), RAL 2021, [[bilibili]](https://www.bilibili.com/video/BV1sq4y1779e/)


<section id="flight-control"></section>

## 3.3 Flight Control 飞行控制

todo

<section id="exploration"></section>

## 3.4 Exploration 探索

todo

* [RACER: Rapid Collaborative Exploration With a Decentralized Multi-UAV System](https://ieeexplore.ieee.org/document/10038280), [[code]](https://github.com/SYSU-STAR/RACER), TRO 2023, 周指导也一直在做这方面的工作

<section id="swarm"></section>

## 3.5 Swarm 集群

涉及到编队，协同飞行等：

* [Swarm of micro flying robots in the wild](https://www.science.org/doi/10.1126/scirobotics.abm5954),Science Robotics 2023, Fast Lab ZJU, 即使你不做无人机，可能都听说过这篇
* [Primitive-Swarm: An Ultra-lightweight and Scalable Planner for Large-scale Aerial Swarms](https://arxiv.org/abs/2502.16887), TRO 2025, [[bilibili]](https://www.bilibili.com/video/BV1Q4PNeeE7D/)
* [EGO-Swarm: A Fully Autonomous and Decentralized Quadrotor Swarm System in Cluttered Environments](https://ieeexplore.ieee.org/document/9561902), ICRA 2021, [[bilibili]](https://www.bilibili.com/video/BV1Nt4y1e7KD/)
* [Distributed Swarm Trajectory Optimization for Formation Flight in Dense](https://ieeexplore.ieee.org/document/9812050), ICRA 2022, [[bilibili]](https://www.bilibili.com/video/BV1qv41137Si)

<section id="state-estimation"></section>

## 3.6 State Estimation 状态估计

空中机器人的状态估计问题在于通过传感器观测数据和控制输入，在噪声干扰下推断机器人位姿、环境特征位置等。SLAM技术中，机器人不仅需要实时定位自身位姿，还需同步构建环境地图。

根据传感器类型来划分：

- 激光SLAM（激光雷达，有机械式和固态式激光雷达）
  - [Zhang, J., & Singh, S. (2014). *LOAM: Lidar Odometry and Mapping in Real-time*. Robotics: Science and Systems (RSS)](https://www.ri.cmu.edu/pub_files/2014/7/Ji_LidarMapping_RSS2014_v8.pdf) 经典的机械式激光雷达算法，将激光雷达里程计与建图分离的框架。
  - [Shan, Tixiao, and Brendan Englot. "Lego-loam: Lightweight and ground-optimized lidar odometry and mapping on variable terrain." *2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*. IEEE, 2018.](https://ieeexplore.ieee.org/abstract/document/8594299)LOAM基础上增加了优化特征匹配和引入闭环检测。
  - [Shan, Tixiao, et al. "Lio-sam: Tightly-coupled lidar inertial odometry via smoothing and mapping." *2020 IEEE/RSJ international conference on intelligent robots and systems (IROS)*. IEEE, 2020.](https://ieeexplore.ieee.org/abstract/document/9341176/)结合激光雷达与IMU的紧耦合方法，通过因子图优化提升大规模场景的鲁棒性。
  - [Xu, Wei, and Fu Zhang. "Fast-lio: A fast, robust lidar-inertial odometry package by tightly-coupled iterated kalman filter." *IEEE Robotics and Automation Letters* 6.2 (2021): 3317-3324.](https://ieeexplore.ieee.org/abstract/document/9372856/) 固态式激光雷达的框架，成本低，速度快。
- 视觉SLAM（单目针孔相机、双目相机、RGB-D深度相机；同时根据方法还可以划分为特征点法，直接法等）
  - [Mur-Artal, R., & Tardós, J. D. (2016). *ORB-SLAM2: An Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras*. IEEE Transactions on Robotics](https://ieeexplore.ieee.org/abstract/document/7946260) ORB-SLAM经典框架，较高的定位精度和框架。此外，还包含了双目、RGB-D相机多重模式。
  - [Engel, Jakob, Thomas Schöps, and Daniel Cremers. "LSD-SLAM: Large-scale direct monocular SLAM." *European conference on computer vision*. Cham: Springer International Publishing, 2014.](https://link.springer.com/chapter/10.1007/978-3-319-10605-2_54) 直接法，支持单目相机的半稠密建图。
  - [Forster, Christian, Matia Pizzoli, and Davide Scaramuzza. "SVO: Fast semi-direct monocular visual odometry." *2014 IEEE international conference on robotics and automation (ICRA)*. IEEE, 2014.](https://ieeexplore.ieee.org/abstract/document/6906584) 半直接法，利用稀疏特征点初始化，再通过直接法优化位姿。
- 多传感器融合（激光雷达、视觉图像、IMU、GPS等多种传感器融合）
  - [Qin, T., Li, P., & Shen, S. (2018). *VINS-Mono: A Robust and Versatile Monocular Visual-Inertial State Estimator*. IEEE Transactions on Robotics](https://ieeexplore.ieee.org/abstract/document/8421746/) 视觉信息与IMU融合的VINS系列，轻量级速度快。
  - [Lin, Jiarong, and Fu Zhang. "R 3 LIVE: A Robust, Real-time, RGB-colored, LiDAR-Inertial-Visual tightly-coupled state Estimation and mapping package." *2022 International Conference on Robotics and Automation (ICRA)*. IEEE, 2022.](https://ieeexplore.ieee.org/abstract/document/9811935/) 融合激光雷达、视觉和IMU，实时构建带颜色的稠密地图。
  - [ORB-SLAM3: An Accurate Open-Source Library for Visual, Visual–Inertial, and Multimap SLAM](https://ieeexplore.ieee.org/document/9440682)，TRO 2020, 支持多传感器融合，并且多地图
  - [GVINS: Tightly Coupled GNSS–Visual–Inertial Fusion for Smooth and Consistent State Estimation](https://ieeexplore.ieee.org/document/9667780), TRO 2022, HKUST Aerial Robotics Group, GNSS + VINS

<section id="aerial-manipulation"></section>

## 3.7 Aerial Manipulation 空中操作

* [Whole-Body Integrated Motion Planning for Aerial Manipulators](https://arxiv.org/abs/2501.06493)

<section id="novel-design"></section>

## 3.8 Novel/Morphing Design 新构型设计/变形无人机

todo



<section id="tech-stack"></section>

# 4. Tech stack 技术栈

<img src="./assets/images/技术栈Aerial RoboticsTech Stack.png" alt="Aerial Robotics Tech Stack" width="800px"/>

<section id="general-design"></section>

## 4.1 General Design 总体设计

总体设计一般是从需求出发，进行设计与分析。

<section id="pure-self-design"></section>

### 4.1.1 Self-Design 自主设计

- CAD设计与仿真：SolidWorks, Fusion 360, CATIA
- 机械结构仿真与分析：ANSYS, ABAQUS
- 快速原型制作：3D打印
- 设计翼型，根据需求确定桨叶升力系数等参数
- 根据需求和重量要求选择电机，电调，桨叶，电池等

<section id="buy-as-need"></section>

### 4.1.2 Buy-as-Needed 采购

根据需求，参考[飞行评测](https://flyeval.com/paper/index.html)与[Fast Drone 250](https://github.com/ZJU-FAST-Lab/Fast-Drone-250)。

<section id="dynamics"></section>

## 4.2 Dynamics 动力学

<section id="fluid mechanics"></section>

### 4.2.1 Fluid Mechanics流体力学

推荐听[余文胜](https://www.aero.sjtu.edu.cn/szdw/szml/27)老师的课。

<section id="aerodynamics"></section>

### 4.2.2 Aerodynamics空气动力学

- 气动建模与分析：XFLR5（简单构型）

<section id="flightdynamics"></section>

### 4.2.3 Flight Dynamics飞行力学

<section id="mechanics"></section>

## 4.3 Mechanics 机械

<section id="embedded"></section>

## 4.4 Embedded 嵌入式

<section id="stm32"></section>

### 4.4.1 STM32

<section id="nuttx"></section>

### 4.4.2 NuttX

实时操作系统，支持Pixhawk开源飞控平台

<section id="Pixhawk"></section>

### 4.4.3 Pixhawk

<section id="other-flight-hardware"></section>

### 4.4.4 Other Flight Hardware

<section id="communication"></section>

## 4.5 Communication 通信

<section id="communication-basis"></section>

### 4.5.1 Communication Basics 通信原理

<section id="uart"></section>

### 4.5.2 UART

<section id="CAN"></section>

### 4.5.3 CAN

<section id="ROS"></section>

### 4.5.4 ROS及功能包

<section id="sensing"></section>

## 4.6 Sensing/Perception 传感/感知

<section id="sensors"></section>

### 4.6.1 Sensors 传感器

<section id="sensing/state-estimation"></section>

### 4.6.2 State Estimation 状态估计

<section id="tracking"></section>

### 4.6.3 Tracking 目标跟踪

<section id="control"></section>

## 4.7 Control 控制

<section id="control-basis"></section>

### 4.7.1 Control Basics 控制原理

<section id="control-methods"></section>

### 4.7.2 Control Methods 控制方法

<section id="control-architecture"></section>

### 4.7.3 PX4-Autopilot PX4飞控

官方资源：

* [github repo: PX4-Autopilot](https://github.com/PX4/PX4-Autopilot)
* [discussion forum](https://discuss.px4.io/)
* [PX4 Guide](https://docs.px4.io/main/en/)
* [discord](https://discord.com/channels/1022170275984457759/1022185721450213396)

推荐走issue和discord两条路，论坛基本没人看也没人回复。相比之下，discord更活跃一些，channels也比较全面。另外一定要多看doc，其实很多东西已经写在里面了（注意看对应版本的，会有很多参数的定义变化，比如`EKF2_AID_MASK`与`EV_CTRL`）。

其他资源:

* [github repo: potato77的笔记](https://github.com/potato77/Tech_Blog/tree/master)
* [XTDrone](https://www.yuque.com/xtdrone/manual_cn)，全面的仿真与算法验证平台，非常适合上手；注意用的是二次开发的基于1.13版本的PX4
* [PegasusSimulator](https://pegasussimulator.github.io/PegasusSimulator/), PX4与Issac Sim结合，但是目前只支持到MC
* [AirGym](https://github.com/emNavi/AirGym), 基于Issac Gym的PX4+RL训练仿真

PX4的版本不是越新越好，大家普遍用的还是1.13，尽管后续版本出了很多功能；但是如果你能接受1.13里混乱的mixer，这个版本的issue与debug信息应该是最多的。

PX4的clone与编译可以参考[make px4](https://jaimeparker.github.io/tech/Make-PX4/)。

如果只是对控制算法或某个模块算法进行改进，那么你需要c++的继承派生虚函数等知识（写的很优雅，其实叫自动驾驶仪，飞控窄了）；如果是对飞控的整体架构进行改进，那么你需要了解PX4的整体架构，尤其是模块间的通信机制。

<section id="optimal-control-optimization"></section>

### 4.7.4 Optimal Control and Optimization 最优控制与优化

(来自于科研时长两年半的硕士升博士生，主要研究中包含间接法最优控制）

#### 4.7.4.1 Introduction 简要概述

最优控制方法主要分成间接法最优控制和直接法最优控制。间接法和直接法最主要的区别我认为是是否引入协态变量以及是否把各个时间点离散出来（直接法中的单次打靶法除外），具体来说直接法会需要把初始时刻、终端时刻、以及中间部分时间节点的状态（有时候也会把控制量拎出来）结合起来形成一个巨大的状态矩阵。除此之外，最优控制问题和一般的优化问题的主要区别在于，最优控制问题需要考虑动力学方程或者是运动学方程，它是作为一个全时间段上的约束存在的。

#### 4.7.4.2 Indirect Method 间接法

推荐书籍：飞行器最优控制 —— 西工大出版社、Optimal Control with Engineering Application（Hans.P.Geering）

* 间接法最优控制主要是以变分法（Variation）为基础，庞特里亚金极大值（也有说是极小值的）原理为理论指导的最优控制方法，优势在于其得出的解一定符合一阶最优性条件（即一定是极值点），缺点在于协态初值需要猜，而且全局最优解和这个猜的初值有关（即不一定是最值点）。
* 具体推导可以看《飞行器最优控制》（毕竟是中文版，遇到不懂的再看后面那本，前者基本上讲的很清楚），引入了协态量，从我的视角来看它就是并列于状态量的一个概念（所以英文叫costate），然后围绕状态量和协态量有一个微分方程组，即一个augmented的动力学方程。除此之外，围绕一阶最优性条件会导出很多关于协态的边界条件（称为横截条件transversal condition），再加上原本状态量的约束，就构成了所有的边界条件。另外，控制量可以基于一阶最优性条件，使得哈密顿函数取到极大值来得到（一般存在解析解，是可以用协态和状态表达的）。如此以后，就成功地把求最优的问题改写成了一个普通的求初始值（初始的协态和状态，需要猜）的问题。另外，如果有等式形式的初始和终端状态约束，比如x+y=R（R为常数）这种，《飞行器最优控制》这本书也有提到，能够很方便的引入刚刚转化好的方程中。
* 当整个优化过程有全时间域的路径约束（比如x>R）这种，可以看第二本书，这本书的第二章有具体推导，可以看一下。

#### 4.7.4.3 Direct Method 直接法

* 直接法的话我了解的不是很多，主要是跟着学校的课程学的
* [直接法的分类](https://blog.csdn.net/Ruins_LEE/article/details/125681168)，对直接法的各个类别有非常详细的分类，肯定比我厉害。

#### 4.7.4.4 常见的优化算法

另外我想在这补充一些常见的优化算法以及用这些算法的C++和Matlab库，虽然现在的包啊库啊整合的都挺好，但是有一些底层的原理如果有感兴趣的也可以自己去看一看。

* [Levenberg-Marquardt 算法](https://blog.csdn.net/weixin_45498383/article/details/143435177)：用于Minpack（C++）、Ceres Solver（C++）、fsolve（Matlab）
* [Powell的dogleg方法](https://blog.csdn.net/woyaomaishu2/article/details/135686350?spm=1001.2014.3001.5501)：用于Minpack（C++）、fsolve（Matlab）
* [Nelder-Mead单纯形法](https://blog.csdn.net/weixin_52732185/article/details/129105796)：用于OptimLib（C++）、fminsearch（Matlab）
* [Trust-Region Reflective方法]()：用于Ceres Solver（C++）、fsolve（Matlab）、fminunc（Matlab）、fmincon（Matlab）
* [BFGS拟牛顿法,L-BFGS拟牛顿法（省内存）等各种拟牛顿法](https://blog.csdn.net/songbinxu/article/details/79677948)：用于NLopt（C++）、OptimLib（C++）、dlib（C++）

当然，这些只是目前我看的一些，只是之前科研的时候突然感兴趣简单搜索了一下，肯定还有很多别的算法，感兴趣的话可以在这里补充。

最优控制说到底是一个优化问题，拿到解析解或数值解（数值优化方法）。另外机器人学的数值优化推荐看汪博在深蓝学院讲的。

<section id="planning"></section>

## 4.8 Planning 规划

推荐课程：[移动机器人运动规划](https://www.shenlanxueyuan.com/course/633?source=1)

<section id="path-planning"></section>

### 4.8.1 Path Planning 路径规划

一定要区分path和trajectory，path是空间上依次排列的点集，而trajectory是时间参数化后的，时间的函数。

<section id="trajectory-planning"></section>

### 4.8.2 Trajectory Planning 轨迹规划

<section id="motion-planning"></section>

### 4.8.3 Motion Planning 运动规划

<section id="task-planning"></section>

### 4.8.4 Task Planning 任务规划

<section id="simulation"></section>

## 4.9 Simulation 仿真

<section id="gazebo"></section>

### 4.9.1 Gazebo

<section id="air-sim"></section>

### 4.9.2 AirSim

<section id="Flightmare"></section>

### 4.9.3 Flightmare

<section id="Rotors-simulation"></section>

### 4.9.4 Rotors Simulation

<section id="Issac-Sim"></section>

### 4.9.5 Isaac Sim

- [IsaacSim](https://github.com/isaac-sim)
- [IsaacSim Documentation](https://docs.isaacsim.omniverse.nvidia.com/latest/index.html)

#### 4.9.5.1 安装配置
- 官方教程：
  - [Installation](https://docs.isaacsim.omniverse.nvidia.com/latest/installation/index.html)
  - 这个安装教程看着有点麻烦，其实如果主要是使用IsaacLab进行训练，可以直接看isaaclab documentation里面的isaacsim安装部分，简单明了。
- 注意事项：
  - 建议下载asset在本地部署
      - [Setup Tips](https://docs.isaacsim.omniverse.nvidia.com/latest/installation/install_faq.html)
  - 第一次运行isaacsim一般都会卡住然后显示isaacsim no responding，一般就是等一段时间或者重新启动几次就会好。

#### 4.9.5.2 IsaacLab
- Isaac Lab 是基于 NVIDIA Isaac Sim 构建的一个开源机器人学习与控制研究平台，主要用于做RL训练。
  - [IsaacLab](https://github.com/isaac-sim/IsaacLab)
  - [IsaacLab Documentation](https://isaac-sim.github.io/IsaacLab/main/index.html)
- 安装：
  - [Local Installation](https://isaac-sim.github.io/IsaacLab/main/source/setup/installation/index.html)
- 环境：
  - [Available Environments](https://isaac-sim.github.io/IsaacLab/main/source/overview/environments.html)
  - 环境类型：
    - Manager-based: 模块化、可扩展、结构化的工作流，适合构建复杂环境、多个组件协同工作的仿真任务。
    - Direct Workflow: 更加灵活，从底层对环境进行定义。一般自定义环境用direct workflow较多，但是缺点是不便于维护和协作，不适合做大项目。

#### 4.9.5.3 相关资源（非官方）
- [Attic IsaacSim-IsaacLab安装注意事项](https://osaerialrobot.top/2025/04/30/IssacSim-IsaacLab/)
- [isaac-sim/IsaacLab | DeepWiki](https://deepwiki.com/isaac-sim/IsaacLab)


<section id="Aerial-Gym"></section>

### 4.9.6 Aerial Gym

* [AirGym](https://github.com/emNavi/AirGym)
* [Aerial Gym Simulator](https://github.com/ntnu-arl/aerial_gym_simulator)

<section id="real-flight"></section>

## 4.10 Real Flight 实机

<section id="remote-control"></section>

### 4.10.1 Remote Control 遥控

<section id="QGC"></section>

### 4.10.2 QGC

<section id="flight-log"></section>

### 4.10.3 Flight Log 飞行日志

什么？你不看飞行日志？

PX4官网有专门的介绍：[Flight Log Analysis](https://docs.px4.io/main/en/log/flight_log_analysis.html)

在这些工具之中，我强推[Plotjuggler](https://docs.px4.io/main/en/log/flight_log_analysis.html)(Grazie Davide Faconti!)：

* 跨平台，linux上体验更好，可以和ros联动，你会爱上他的republish功能的
* 每次打开都有奇奇怪怪的图
* 还有教程，支持插件，[github](https://github.com/facontidavide/PlotJuggler)

<section id="companion-computer"></section>

### 4.10.4 Companion Computer 上位机

<section id="nn-methods"></section>

## 4.11 NN Methods learning方法

<section id="reinforcement-learning"></section>

### 4.11.1 Reinforcement Learning 强化学习

<section id="generative-models"></section>

### 4.11.2 Generative Models 生成模型

<section id="LLM"></section>

### 4.11.3 (M)LLMs （视觉等模态）大语言模型


<section id="labs-home"></section>

# 5. Labs and Homepages

<section id="domestic"></section>

注：所有顺序无意义 

## 5.1 Domestic(PRC) 国内

<section id="chinamainland"></section>

### 5.1.1 Mainland PRC 中国大陆

* [Fast Lab ZJU](http://zju-fast.com/)
* [可靠飞行控制研究组 BUAA](https://shi.buaa.edu.cn/quanquan/zh_CN/index/4733/list/index.htm)
* [郭雷 BUAA](https://shi.buaa.edu.cn/guolei/zh_CN/)
* [IRMV Lab SJTU](http://irmv.sjtu.edu.cn/)
* [Shanghai Key Lab of Navigation & Location-based Services SJTU](https://drone.sjtu.edu.cn/dpzou/)
* [董伟 SJTU](https://me.sjtu.edu.cn/teacher_directory1/dongwei1.html)
* [STAR SUSTech](https://robotics-star.com/)
* [田栢苓 TJU](https://faculty.tju.edu.cn/116115/zh_CN/index.htm)
* [WINDY Lab](https://shiyuzhao.westlake.edu.cn/)
* [吕熙敏 SYSU](https://scholar.google.com/citations?user=obB-btEAAAAJ&hl=en)
* [RAPID Lab SYSU](http://lab.sysu-robotics.com/index.html)
* [NICSefc THU](https://nicsefc.ee.tsinghua.edu.cn/) MARL小组，于超老师，xhs id 94742231017
* [NPU-IUS-Lab](https://space.bilibili.com/1379550426?spm_id_from=333.1387.follow.user_card.click)
* [王耀南 院士](https://eeit.hnu.edu.cn/info/1277/4490.htm)
* [夏元清](https://pure.bit.edu.cn/zh/persons/yuanqing-xia)
* [HNU-CAT](https://space.bilibili.com/3546815712462924?spm_id_from=333.1387.follow.user_card.click)
* [孟伟](https://space.bilibili.com/403212208?spm_id_from=333.1387.follow.user_card.click)


<section id="hongkong"></section>

### 5.1.2 Hongkong, China 中国香港

* [HKUST Aerial Robotics Group](https://uav.hkust.edu.hk/)
* [MaRS Lab HKU](https://mars.hku.hk/)
* [ArcLab HKU](https://arclab.hku.hk/)
* [AIMS PolyU](https://sites.google.com/view/hailong-huang/home)


<section id="overseas"></section>

## 5.2 Overseas(Out of PRC) 国外

<section id="north-america"></section>

### 5.2.1 North America 北美

* [GRASP Laboratory UPenn](https://www.grasp.upenn.edu/), **[Vijay Kumar](https://www.kumarrobotics.org/)**
* [HiPeRLab UC Berkeley](https://hiperlab.berkeley.edu/)
* [AirLab CMU](https://theairlab.org/)
* [LECAR Lab CMU](https://lecar-lab.github.io/)
* [Russ Tedrake](https://locomotion.csail.mit.edu/russt.html)
* [MIT Aerospace Controls Laboratory](https://acl.mit.edu/)

<section id="europe"></section>

### 5.2.2 Europe 欧洲

* [ETH ASL](https://asl.ethz.ch/)
* [RPG UZH](https://rpg.ifi.uzh.ch/)
* [MAVLab TUDelft](https://mavlab.tudelft.nl/)
* [V4RL ETH](https://www.v4rl.com/)


<section id="asia"></section>

### 5.2.3 Asia 亚洲

* [Dragon Lab 东京大学](http://www.dragon.t.u-tokyo.ac.jp/)
* [谢立华 NTU](https://personal.ntu.edu.sg/elhxie/)
* [Unmanned Systems Research Group CUHK&NUS](http://www.mae.cuhk.edu.hk/~usr/index.html)
* [AIRS NTU](https://ntu-aris.github.io/), [bilibili](https://space.bilibili.com/313085009?spm_id_from=333.1387.follow.user_card.click)
* [ICG NTU](https://sites.google.com/view/mir-feroskhan/about)

