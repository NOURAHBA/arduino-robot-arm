# arduino-robot-arm
 install  arduino robot arm packages to control  robot arm with Moveit and Rviz
 ## Create a catkin workspace
 Before start creating and building arduino robot arm packages , must first create a ROS workspace folder by follow These instructions in terminal
 
 `$ mkdir -p ~/catkin_ws/src`
 
`$ cd ~/catkin_ws/`

`$ catkin_make`


at the end of the (bashrc) file add the follwing line
(source /home/(your user name )/catkin_ws/devel/setup.bash)
then 
ctrl + o
##  install  arduino robot arm packages
follow These instructions in terminal

`cd ~/catkin_ws`

`rosdep install --from-paths src --ignore-src -r -y`

`sudo apt-get install ros-melodic-moveit`

`sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui`

`sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher`

`sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control`

## Simulation
Run the following instructions to use gazebo Rivz

`roslaunch robot_arm_pkg check_motors.launch`

default positions

<img width="596" alt="Capture" src="https://user-images.githubusercontent.com/86157318/122808699-e2cec200-d2d5-11eb-9f8c-ad4a7bd89c27.PNG">

positions after change

<img width="595" alt="Capture1" src="https://user-images.githubusercontent.com/86157318/122808866-13166080-d2d6-11eb-9586-ea95774843ea.PNG">

