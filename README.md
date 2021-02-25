#ROS executable to run two turtlesims concurrently using both a keyboard and an xinput controller

Requirements to run:
A keyboard and xinput joystick*
Twist Keyboard: http://wiki.ros.org/teleop_twist_keyboard
Twist Joy: http://wiki.ros.org/teleop_twist_joy

*Most controllers support xinput. It's worth noting that a controller doesn't have to be installed to execute the program, however you will of course be unable to test if both inputs are working.

Copy this repository to your work space's source folder

Steps to run:
Terminal 0: $ roscore
Terminal 1: Source and build your workspace 
(eg: 
$ source devel/setup.bash 
$ catkin_make
or
$ source devel/setup.bash 
$ catkin build)

Terminal 1: $ cd ~/[YOUR WORKSPACE]/src/twoirtoise 

To test concurrent inputs:
$ roslaunch twoirtoise_sim.launch
You'll be able to drive both robots with the two separate input devices

To start a basic turtlesim:
Terminal 1: Launch tortoise_sim.launch to start a launchable version of the command line turtlesim found at http://wiki.ros.org/ROS/Tutorials/UnderstandingNodes


