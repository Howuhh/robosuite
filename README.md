# robosuite

![gallery of_environments](docs/images/gallery.png)

**robosuite** is a robotic simulation library powered by the [MuJoCo physics engine](http://mujoco.org/) for accessible and reproducible robot learning research. The current release focuses on robot manipulation. **robosuite** is part of the broader Advancing Robot Intelligence through Simulated Environments (ARISE) Initiative.

Data-driven algorithms, such as reinforcement learning and imitation learning, provide a powerful and generic tool in robotics. These learning paradigms, fueled by new advances in deep learning, have achieved some exciting successes in a variety of robot control problems. However, the challenges of reproducibility and the limited accessibility of robot hardware (especially during a pandemic) have impaired research progress. The overarching goal of **robosuite** is to provide researchers with:

* a standardized set of benchmarking tasks for rigorus evaluation and algorithm development;
* a modular design that offers great flexibility to design new robot simulation environments;
* a high-quality implementation of robot controllers and off-the-shelf learning algorithms to lower the barriers to entry.

This library was originally developed since late 2017 by researchers in [Stanford Vision and Learning Lab](http://svl.stanford.edu/) (SVL) as an internal tool for robot learning research. Now it is actively maintained and used for robotics research projects in SVL and the Robot Perception and Learning (RPL) Lab at UT-Austin.

This release of **robosuite** contains seven robot models, eight gripper models, six controller modes, and nine standardized tasks. It also offers a modular design of APIs for building new environments with procedural generation. We highlight these primary features below:

* [**standardized tasks**](modules/environments): a set of standardized manipulation tasks of large diversity and varying complexity and RL benchmarking results for reproducible research;
* [**procedural generation**](modules/overview): modular APIs for programmatically creating new environments and new tasks as a combinations of robot models, arenas, and parameterized 3D objects;
* [**controller supports**](modules/controllers): a selection of controller types to command the robots, such as joint-space velocity control, inverse kinematics control, operational space control, and 3D motion devices for teleoperation;
* [**multi-modal sensors**](modules/sensors): heterogeneous types of sensory signals, including low-level physical states, RGB cameras, depth maps, and proprioception;
* [**human demonstrations**](algorithms/demonstrations): utilities for collecting human demonstrations, replaying demonstration datasets, and leveraging demonstration data for learning.


## Citations
Please cite [robosuite](http://surreal.stanford.edu) if you use this library in your publications:
```
@inproceedings{corl2018surreal,
  title={SURREAL: Open-Source Reinforcement Learning Framework and Robot Manipulation Benchmark},
  author={Fan, Linxi and Zhu, Yuke and Zhu, Jiren and Liu, Zihua and Zeng, Orien and Gupta, Anchit and Creus-Costa, Joan and Savarese, Silvio and Fei-Fei, Li},
  booktitle={Conference on Robot Learning},
  year={2018}
}
```
