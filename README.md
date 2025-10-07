# Greeting-Robot-TNTech-2025-Rover
Tracklist of the Fall 2025 Senior Design group working on Rover

## Starting Rover from the Intel NUC in the base
Make sure the computer is on by pressing the square button located on the
back of the computer.

Open a terminal by pressing Ctrl + Alt + T. From there, enter the following in the rover@rover/ros2_ws folder: 
- source install/setup.bash ros2 launch 
- roverrobotics_driver pro.launch.py

# Sending cmd_vel using ROS2 Topic
cmd_vel is what keeps track of the movement of Rover. This section is useful for testing whether and motors in rover are still responsive to code as well as to check whether they need replacing/upgrading.

Enter the following in the rover@rover/ros2_ws folder:
