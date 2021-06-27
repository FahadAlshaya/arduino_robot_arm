# arduino_robot_arm
ROS packages that can be used to plan and execute motion trajectories for a robot arm in simulation and real-life.

for use the packages i use Ros Melodic and ubuntu-18.04 after installing it, you need to create a workspace.

run this instruction to creat your  workspace:

- [$ source /opt/ros/noetic/setup.bash]()
- [$ mkdir -p ~/catkin_ws/src]()
- [$ cd ~/catkin_ws/]()
- [$ catkin_make]()


# Installing the package arduino_robot_arm
run this instruction inside your workspace:
	$ cd ~/catkin_ws/src
	$ sudo apt install git
	$ git clone https://github.com/smart-methods/arduino_robot_arm 
	$ cd ~/catkin_ws
	$ rosdep install --from-paths src --ignore-src -r -y
	$ sudo apt-get install ros-melodic-moveit
  $ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
  $ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
  $ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control


# Compile the package
  $ catkin_make
  
 
 # Controlling the motors
 $ roslaunch robot_arm_pkg check_motors.launch

 
 ![robot_arm](https://user-images.githubusercontent.com/60845044/123549884-8b1bd500-d773-11eb-94eb-c1751da126c9.png)

 






