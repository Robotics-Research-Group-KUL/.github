# 🦾 Software at the Robotics Group (KU Leuven)

## 🤖 eTaSL-related packages

### eTaSL for ROS2

| Package                            | Description                                                      |
| ---------------------------------- | ---------------------------------------------------------------- |
| ├─ [`etasl_ros2`](https://github.com/Robotics-Research-Group-KUL/rttlua_completion) | Enables tab completion in the `rttlua` shell                     |

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
