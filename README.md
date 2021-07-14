<img width="459" alt="Screen Shot 1442-12-04 at 8 36 53 AM" src="https://user-images.githubusercontent.com/86019166/125591104-49ff5b69-84bc-4b42-b328-4263a3a5b470.png"><img width="664" alt="Screen Shot 1442-12-04 at 11 36 23 AM" src="https://user-images.githubusercontent.com/86019166/125591120-8d2bd735-4576-4da2-9d35-c732b104a6ee.png">
<img width="444" alt="Screen Shot 1442-12-04 at 11 35 01 AM" src="https://user-images.githubusercontent.com/86019166/125591125-674d3e73-4f46-4d5e-af48-d8e23550f75c.png">

Navigation Simulation

1/Launch Simulation World
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch

2/Run Navigation Node
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml

3/Estimate Initial Pose
3.1/Click the 2D Pose Estimate button in the RViz menu.
3.2/Click on the map where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.
3.3/Repeat step 1 and 2 until the LDS sensor data is overlayed on the saved map.
3.4/Launch keyboard teleoperation node to precisely locate the robot on the map.
$ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch.
3.4/Move the robot back and forth a bit to collect the surrounding environment information and narrow down the estimated location of the TurtleBot3 on the map which is displayed with tiny green arrows.
3.5/Terminate the keyboard teleoperation node by entering Ctrl + C.

4/Set Navigation Goal
4.1/Click the 2D Nav Goal button in the RViz menu.
4.2/Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing.

<img width="664" alt="Screen Shot 1442-12-04 at 11 36 23 AM" src="https://user-images.githubusercontent.com/86019166/125591216-5e4fb354-cd85-4271-a116-68ca76e1afe4.png">
<img width="459" alt="Screen Shot 1442-12-04 at 8 36 53 AM" src="https://user-images.githubusercontent.com/86019166/125591231-c0edc050-747a-4f46-899e-07321f0c7d4d.png">
<img width="444" alt="Screen Shot 1442-12-04 at 11 35 01 AM" src="https://user-images.githubusercontent.com/86019166/125591237-edabb2e8-dedb-4ec5-876c-f48ebf3b1d3b.png">
