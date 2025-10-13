# Greeting-Robot-TNTech-2025-Rover

# Getting Started on Rover:

## Starting Rover from the Intel NUC in the base
Make sure the computer is on by pressing the square button located on the
back of the Intel NUC located in the base of the robot.

Open a Linux terminal by pressing Ctrl + Alt + T on the keyboard. From there, enter the following in the rover@rover/ros2_ws directory (if unsure how to change directories, see the following):
- cd ros2_ws ("cd" stands for "Change Directory." This line of code changes the directory to "ros2_ws")
- source install/setup.bash ros2 launch 
- roverrobotics_driver pro.launch.py

## Sending cmd_vel using ROS2 Topic
cmd_vel is what keeps track of the movement of Rover. This section is useful for testing whether and motors in Rover are still responsive to code as well as to check whether they need replacing/upgrading.

Enter the following in the rover@rover/ros2_ws directory: 
- topic pub /cmd_vel geometry_msgs/msg/Twist '{linear: {x: 0.5, y: 0.0, z: 0.0}}' -r 10 

## Sending cmd_vel using Joystick
Rover has the ability to be placed into Manual Mode. While in this mode, the robot can be controlled via Playstation 4 controller. To pair the controller, press and hold the Playstation button until the light blinks blue. Then, on Rover's screen, click the settings button in the top right and select "Bluetooth." From there, connect the "Wireless Controller" device. 

From there, open another terminal window and enter the following in the rover@rover/ros2_ws directory: 
- launch roverrobotics_driver ps4_controller.launch.py
