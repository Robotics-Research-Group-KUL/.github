# 🦾 Software at the Robotics Group (KU Leuven)

## 🤖 Crospi: Constraint-based Reactive and Orchestrated Sensor-driven PIpeline.

Crospi is a highly-configurable pipeline that focuses on interfacing (plugins, ROS2 and non-ROS sensors, robot hardware, easy user interfaces) and easy integration (pipeline for Orchestration, creation of libraries, configuration files, etc).  It uses eTaSL which is a  collection of C++/CMake/LUA libraries taht define a language and interpreter to specify constraint-based control task specifications. Besides Crospi, there are several other frameworks that use eTaSL, such as ROS/Orocos and ROS2/Orocos (see below). Note that, although the constraint-based task specifications are specified using a scripting language, all real-time critical runs in C++.  With Crospi, you can focus on configuring to use your own robot setup in your own orchestrated applications, and easily reuse tasks and skills from libraries.

| Package                            | Description                                                      |
| ---------------------------------- | ---------------------------------------------------------------- |
| [`crospi_core`](https://github.com/Robotics-Research-Group-KUL/crospi_core) ([`doc`](https://crospi-website-907f83.pages.gitlab.kuleuven.be/)) | This package was created to be able to develop constraint-based reactive robot behaviors with eTaSL that can fully operate with the ROS2 architecture. |
| [`BeTFSM`](https://github.com/Robotics-Research-Group-KUL/betfsm) ([`doc`](https://betfsm-90d316.pages.gitlab.kuleuven.be/)) | BeTFSM is a library for "ticking" statemachines and behavior trees. It targets discrete coordination of robotic systems at both high- and low level.|
| [`crospi_application_template`](https://github.com/Robotics-Research-Group-KUL/crospi_application_template) | This is a template that facilitates development and provides development functionalities to speed up development and deployment with Crospi.                     |
| [`crospi_default_plugins`](https://github.com/Robotics-Research-Group-KUL/crospi_default_plugins) | This package contains the default plugins for crospi_core.                     |
| [`crospi_interfaces`](https://github.com/Robotics-Research-Group-KUL/crospi_interfaces) | Package containing ros msgs and srv used to communicate with the crospi_core package. |
| [`skill_lib_example`](https://github.com/Robotics-Research-Group-KUL/skill_lib_example) | Package with an example of a skill for Crospi. This contains BetFSM skill orchestration examples. |
| [`core_task_lib`](https://github.com/Robotics-Research-Group-KUL/core_task_lib) | Package with core and common eTaSL task specifications that can be used within the Crospi pipeline for controlling robots. |
| [`debug_lib`](https://github.com/Robotics-Research-Group-KUL/debug_lib) | Package with eTaSL task specifications for debugging that can be used within the Crospi pipeline. |
| [`dummy_lib`](https://github.com/Robotics-Research-Group-KUL/dummy_lib) | Package with dummy examples of eTaSL task specifications that can be used within the Crospi pipeline. |
| [`template_driver_crospi`](https://github.com/Robotics-Research-Group-KUL/template_driver_crospi) | This package contains a template on how to implement a robot driver for crospi_core node using ROS2 plugins. If used without any modification, it will simply simulate the robot by integrating the joint velocities and returning joint positions through shared memory communication. |
| [`kuka_iiwa_driver_crospi`](https://github.com/Robotics-Research-Group-KUL/kuka_iiwa_driver_crospi) | This package contains a driver for controlling the Kuka iiwa using crospi_core, based on template_driver_crospi package which uses ROS2 plugins. |
| [`expressiongraph`](https://github.com/Robotics-Research-Group-KUL/expressiongraph) | This package contains a library for automatic differentiation specifically targeted to robotics data-types such as orientations, quaternions, poses, twists and wrenches |
| [`luabind`](https://github.com/Robotics-Research-Group-KUL/luabind) | This package contains C++ template utilities to bind C++ code to lua |
---

## 🧩 Orocos and rtt-ros Packages

While Orocos is nowadays maintained externally, we keep some packages that can prove useful:

### rtt-ros for ROS1 (Noetic)

| Package                            | Description                                                      |
| ---------------------------------- | ---------------------------------------------------------------- |
| [**rtt_ros_utilities**](https://github.com/Robotics-Research-Group-KUL/rtt_ros_utilities)  | A meta-package containing the following packages:       |
| ├─ [`rttlua_completion`](https://github.com/Robotics-Research-Group-KUL/rttlua_completion) | Enables tab completion in the `rttlua` shell                     |
| ├─ [`rFSM`](https://github.com/Robotics-Research-Group-KUL/rFSM)              | State machine framework for Lua                                  |
| ├─ [`rtt_dot_service`](https://github.com/Robotics-Research-Group-KUL/rtt_dot_service)   | Creates a DOT graph from the current deployment                  |
| [**python_gui**](https://github.com/Robotics-Research-Group-KUL/python_gui)         | Configurable ROS graphical interface to send events to `rFSM`    |
| [**URDriver**](https://github.com/Robotics-Research-Group-KUL/URDriver)           | Drivers for using UR robots with ROS                             |
| [**rtt_soem**](https://github.com/Robotics-Research-Group-KUL/rtt_soem)           | EtherCAT master component with plugins (mainly Beckhoff modules) |
| [**rtt_soem_maxpos**](https://github.com/Robotics-Research-Group-KUL/rtt_soem_maxpos)    | EtherCAT drivers for the MaxPos, a motor driver from Maxon motors                 |


### rtt-ros for ROS2 (Foxy)

| Package                            | Description                                                        |
| ---------------------------------- | ------------------------------------------------------------------ |
| [**rtt_ros2_utilities**](URL_HERE) | A meta package containing the following packages:                  |
| ├─ [`motion_control`](https://github.com/Robotics-Research-Group-KUL/motion_control/tree/ros2)    | Legacy message types *(ros2 branch)*                               |
| ├─ [`rFSM`](https://github.com/Robotics-Research-Group-KUL/rFSM/tree/ros2)              | State machine framework *(ros2 branch)*                            |
| ├─ [`ros2_rtt_typekits`](https://github.com/Robotics-Research-Group-KUL/ros2_rtt_typekits) | Typekits for Eigen and KDL                                         |
| ├─ [`rtt_dot_service`](https://github.com/Robotics-Research-Group-KUL/rtt_dot_service/tree/ros2)   | Generates DOT graphs *(ros2 branch)*                               |
| ├─ [`rttlua_completion`](https://github.com/Robotics-Research-Group-KUL/rttlua_completion/tree/ros2) | Lua shell tab completion *(ros2 branch)*                           |
| [**rtt_ros2_pkg**](https://github.com/Robotics-Research-Group-KUL/rtt_ros2_pkg)       | Adds commands for creating Orocos packages in rtt-ros2 integration |
| [**python_gui_ros2**](https://github.com/Robotics-Research-Group-KUL/python_gui_ros2)    | Configurable ROS2 graphical interface to send events to `rFSM`     |
| [**soem**](https://github.com/Robotics-Research-Group-KUL/soem/tree/foxy-devel)               | ROS2 EtherCAT dependency *(use the `foxy_devel` branch)*           |
| [**rtt_soem**](https://github.com/Robotics-Research-Group-KUL/rtt_soem/tree/ros2)           | EtherCAT master component with plugins (mainly Beckhoff modules) *(ros2 branch)*                          |

---

## 🐳 Docker Images

Prebuilt Docker images for ROS1 and ROS2 with the above utilities installed:

👉 [**gborghesan/orocos** on Docker Hub](https://hub.docker.com/r/gborghesan/orocos)



<!--



**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
