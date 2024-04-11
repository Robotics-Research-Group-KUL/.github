# Software at the Robotics Group (KU Leuven)

## Orocos and rtt-ros packages
While Orocos is nowadays maintained externally, we keep some packages that can prove useful
### rtt-ros for ROS1 (noetic)
#### General
- `rtt_ros_utilities`: a meta-package containing the following packages 
  - `rttlua_completion`
  - `rFSM`
  - `rtt_dot_service`
- `python_gui`: a configurable ROS graphical interface to send events to rFSM.
  #### Drivers
- `URDriver`: drivers to to to use UR robots with ROS
- `rtt_soem_maxpos`: ethercat drivers for the MaxPos, a motor driver from Maxon motors.

### rtt-ros for ROS2 (foxy)

- `rtt_ros2_utilities`: a meta package containing the following packages
  -  `motion_control`: legacy message types (__ros2 branch__)
  -  `ros2_rtt_typekits`: typekits for eigen and KDL
  -   `rtt_dot_service`:  (__ros2 branch__)
  -   `rttlua_completion`: (__ros2 branch__)
- `rtt_ros2_pkg`: adding the command to create packages for orocos in rtt-ros2 integration.
- `python_gui_ros2`: a configurable ROS graphical interface to send events to rFSM.


<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
