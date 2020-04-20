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
Launch Nodes:
```
$ roslaunch turtlebot_gazebo turtlebot_world.launch
```
### 2. robot_pose_ekf package:
Clone Package:
```
$ cd /home/workspace/catkin_ws/src/
$ git clone https://github.com/udacity/robot_pose_ekf 
```
Remap the ros topics of turtlebot in the robot_pose_ekf.launch file
Launch Nodes:
```
roslaunch robot_pose_ekf robot_pose_ekf.launch
```
### 3. odom_to_trajectory package:
Clone Package:
```
$ cd /home/workspace/catkin_ws/src
$ git clone https://github.com/udacity/odom_to_trajectory
```
launch the nodes:
```
$ roslaunch odom_to_trajectory create_trajectory.launch 
```
### 4. turlebot_teleop package:
Clone Package:
```
$ cd /home/workspace/catkin_ws/src
$ git clone https://github.com/turtlebot/turtlebot
```
Install the Dependencies:
```
$ cd /home/workspace/catkin_ws
$ source devel/setup.bash
$ rosdep -i install turtlebot_teleop
```

launch the nodes:
```
roslaunch turtlebot_teleop keyboard_teleop.launch
```
### 5. riviz package:
launch the nodes:
run the rviz, add the required things and save the configuration.
create the rviz launch file and run -
```
roslaunch RvizLaunch.launch
```

### create a main package:
```
$ cd /home/workspace/catkin_ws/src
$ catkin_create_pkg main
```
```
roslaunch main main.launch
```
