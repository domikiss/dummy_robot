# dummy_robot

A simple differential robot model for creating dynamic scenarios in ROS/Gazebo (ROS 1)


## Prerequisites

We assume that you have a Desktop-Full installation of ROS, including the Gazebo simulator and `gazebo_ros_pkgs`, the set of packages for interfacing ROS with Gazebo. If you miss any of these, please read the corresponding tutorials:
- [ROS Installation](http://wiki.ros.org/ROS/Installation)
- [Installing gazebo_ros_pkgs (ROS 1)](http://gazebosim.org/tutorials?tut=ros_installing&cat=connect_ros)


## Robot Model

The URDF model of the dummy robot can be found in `dummy_robot_description`. To visualize it in RViz, launch `dummy_robot_rviz.launch`:

```
roslaunch dummy_robot_description dummy_robot_rviz.launch
```
![Dummy robot model](https://domikiss.github.io/dummy_robot/dummy_robot_model.png)


## Simulation

A simple SDF world model `smallroom.world` is provided in `dummy_robot_gazebo`. To simulate the robot in one or more copies in Gazebo, use one of the following roslaunch commands (robots are circling around with constant velocities):

```
roslaunch dummy_robot_gazebo smallroom_1_robot.launch
```
![Gazebo simulation of 1 dummy robot](https://domikiss.github.io/dummy_robot/smallroom_1_robot.png)

```
roslaunch dummy_robot_gazebo smallroom_2_robot.launch
```
![Gazebo simulation of 2 dummy robots](https://domikiss.github.io/dummy_robot/smallroom_2_robot.png)

```
roslaunch dummy_robot_gazebo smallroom_4_robot.launch
```
![Gazebo simulation of 4 dummy robots](https://domikiss.github.io/dummy_robot/smallroom_4_robot.png)

