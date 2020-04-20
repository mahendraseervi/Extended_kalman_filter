# Extended_kalman_filter
Implementaion of Extended Kalman filter to estimate the robot's pose using sensor fusion in the gazebo world

## Ros packages used:
1. turtlebot_gazebo
2. robot_pose_ekf
3. odom_to_trajectory
4. turlebot_teleop
5. rviz

### Turtlebot package:
Clone Package:
```
$ cd /home/workspace/catkin_ws/src
$ git clone https://github.com/turtlebot/turtlebot_simulator
```
Install Dependencies:
```
$ cd /home/workspace/catkin_ws
$ source devel/setup.bash
$ rosdep -i install turtlebot_gazebo
```
Build Package:
```
$ catkin_make
$ source devel/setup.bash
```
Launch Nodes:
```
$ roslaunch turtlebot_gazebo turtlebot_world.launch
```
