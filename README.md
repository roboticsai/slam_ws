1. Launch robot in simulation
roslaunch turtlebot3_gazebo turtlebot3_world.launch
2. Launch slam ros node
roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=hector
3. Launch the controller to move the robot
roslaunch turtlebot3_gazebo turtlebot3_simulation.launch
# slam_ws
