# Extended_kalman_filter
Implementaion of Extended Kalman filter to estimate the robot's pose using sensor fusion (wheel encode, IMU and camera sensor) in the gazebo world

## Ros packages used:
1. turtlebot_gazebo
2. robot_pose_ekf
3. odom_to_trajectory
4. turlebot_teleop
5. rviz

### 1. Turtlebot package:
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

### 2. robot_pose_ekf package:
Clone Package:
```
$ cd /home/workspace/catkin_ws/src/
$ git clone https://github.com/udacity/robot_pose_ekf 
```
Remap the ros topics of turtlebot in the robot_pose_ekf.launch file
