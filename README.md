# BCN3D_Moveo_ROS
# How to Use Moveo_Ros in Ubuntu
Ubuntu 16 (32 bit)
ROS Kinetic 

Install ROS Kinetic 
	http://wiki.ros.org/kinetic/Installation/Ubuntu

Install Arduino IDE (Download from site and ./install.sh)
	https://www.arduino.cc/en/Guide/Linux

Install Arduino library from Arduino IDE (AccelStepper)
Install Arduino library ros_lib
	Download library and:
		cd <sketchbook>/libraries
		rm -rf ros_lib
		rosrun rosserial_arduino make_libraries.py .
	http://wiki.ros.org/rosserial_arduino/Tutorials/Arduino%20IDE%20Setup

Create a ROS Workspace
	$ mkdir -p ~/catkin_ws/src
	$ cd ~/catkin_ws/
	$ catkin_make
	http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment
Copy into ~/catkin_ws/src archive of moveo_ros from GitHub
	https://github.com/jesseweisberg/moveo_ros
Before using terminal for ROS you have to set environment of moveo_ros
	source devel/setup.bash
After that you can execute command from README.md moveo_ros
