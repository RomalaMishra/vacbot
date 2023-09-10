# Vacbot
## A bot which uses LIDAR and designed to map the environment using GMapping

## Installation
### In order to use this package, go through the following steps:

Open you catkin package and go to the src
```bash
cd catkin_ws/src
```
After that clone the repo to your src
```bash
git clone https://github.com/RomalaMishra/Vacbot.git
```
After cloning, source and build the package
```bash
source devel/setup.bash
catkin build
```
## Launching
### In order to launch the package, first launch the gazebo simulation
```bash
roslaunch Vacbot rough.launch
```
Then launch
```bash
roslaunch Vacbot robot_slam.launch
```
This will launch Rviz, which will alllow you to visualise the laserscan and the map obtained

Then run the following script which will allow you to teleop the bot and generate the entire map of the world
```bash
rosrun Vacbot turtlebot3_teleop.py
```
Now move the bot using W,A,S,D keys and see the bot generate a beautifull map of the world.

## Contribution
This project is the result of collaborative efforts. Special thanks to all the contributors who have helped build this project. Contributions to this project are welcome. If you have any ideas for improvements, bug fixes, or additional features, please feel free to fork the repository and submit a pull request.
