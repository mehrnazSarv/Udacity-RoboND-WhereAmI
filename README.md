# Where Am I Project  
This is the 3rd project in the Robotics Software Engineer Nanodegree Program by Udacity.  

## Project Discription  
In this project, I learned several aspects of robotic software engineering with a focus on ROS:  
1. Create a ROS package that launches a custom robot model in a custom Gazebo world  
2. Utilize the ROS AMCL package and the Tele-Operation / Navigation Stack to localize the robot
3. Explore, add, and tune specific parameters corresponding to each package to achieve the best possible localization results  

## Launching   
First, launch the simulation:  
```sh  
$ roslaunch my_robot world.launch
```  

In a new terminal, launch the `amcl` launch file:  
```sh  
$ roslaunch my_robot amcl.launch
```  

## Testing  
There are two options to control my robot while it localize itself here:
  - Send `navigation goal` via RViz
  - Send move command via `teleop` package.  
  
### Option 1: Send `2D Navigation Goal` 
Click the `2D Nav Goal button` in the RViz toolbar, then click and drag on the map to send the goal to the robot. It will start moving and localize itself in the process.  

### Option 2: Use `teleop` Node 
Open another terminal and launch the teleop script:  
```sh
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```  

