## 1. Environment Preparation
OS Installation: I started by installing Ubuntu 22.04.
User Setup: I created my user account sadeemj and ensured I had administrative privileges by adding my user to the sudo group.
ROS 2 Installation: I installed ROS 2 Humble Desktop following the official documentation to include all necessary simulation tools.
![Screenshot (447)](https://github.com/sadeem058/ROS-2-Humble-Setup-and-Turtlesim-Tasks/blob/main/Screenshot%20(447).png)

## 2. Workspace Setup
Every time I start a new session, I initialize my environment using:
**source /opt/ros/humble/setup.bash**

![Screenshot (450)](https://github.com/sadeem058/ROS-2-Humble-Setup-and-Turtlesim-Tasks/blob/main/Screenshot%20(450).png)

## 3. Running Turtlesim
To solve my tasks, I launch the core simulator and the teleoperation tool in separate terminals:
Launch Turtlesim Node: **ros2 run turtlesim turtlesim_node**
Launch Teleop Key: **ros2 run turtlesim turtle_teleop_key**

I used the keyboard arrows and orientation keys (E, B, V, C) to manually navigate the turtle.
By precisely controlling the rotation and forward movement,**I successfully drew a Rhombus (Diamond) shape**.
AND I created STAR by Service Calls for higher precision
**I changed the pen color to Gold using the set_pen service:**

**ros2 service call /turtle1/set_pen turtlesim/srv/SetPen "{r: 255, g: 215, b: 0, width: 5, 'off': 0}"**

**source**

**ros2 service call /turtle1/teleport_relative turtlesim/srv/TeleportRelative "{linear: 2.0, angular: 0.0}"**

**ros2 service call /turtle1/teleport_relative turtlesim/srv/TeleportRelative "{linear: 2.0, angular: 2.513}"**

**ros2 service call /turtle1/teleport_relative turtlesim/srv/TeleportRelative "{linear: 2.0, angular: 2.513}"**

**ros2 service call /turtle1/teleport_relative turtlesim/srv/TeleportRelative "{linear: 2.0, angular: 2.513}"**

**ros2 service call /turtle1/teleport_relative turtlesim/srv/TeleportRelative "{linear: 2.0, angular: 2.513}"**

![Screenshot (451)](https://github.com/sadeem058/ROS-2-Humble-Setup-and-Turtlesim-Tasks/blob/main/Screenshot%20(451).png)
