# ROS-project

## Links
1. [Here](https://www.overleaf.com/5558443539bpxqpnwzqhhh) is the link to latex design document
2. [Here](https://docs.google.com/document/d/1_vgVjlCv3aginC8bU6hgd1d6z14EGoSr1StUOpTOrkk/edit?usp=sharing) is the link to google design document
3. [Here](https://docs.google.com/document/d/1y1RqtI58b2dbTwsi0cbb8ApG6tdWnyAR7fD62_-4gC4/edit?usp=sharing) is the link to google notes document
4. [Diagram](https://drive.google.com/file/d/1gP7IxsNWptns8p6vzZTSO3hJxZwgKq96/view?usp=sharing)
5. [MIR100 github repo](https://github.com/DFKI-NI/mir_robot/tree/noetichttps://github.com/DFKI-NI/mir_robot/tree/noetic)

## Installations
```
$sudo apt install ros-noetic-gmapping
$sudo apt-get install ros-noetic-navigation
$sudo apt-get install ros-noetic-explore-lite
```

## Running

- Launch Gazebo world
```
$roslaunch mir_gazebo mir_maze_world.launch
$rosservice call /gazebo/unpause_physics   # or click the "start" button in the Gazebo GUI
```
- Launch SLAM mapping&localization
```
$roslaunch slam.launch
```
- Save the map
```
$rosrun map_server map_saver -f willo
```
- Localization and path planning
```
to-do
```
- Visualisation
```
$rviz -d $(rospack find mir_navigation)/rviz/navigation.rviz
```
