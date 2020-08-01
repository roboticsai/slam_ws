    Launch the robot in simulation 

roslaunch turtlebot3_gazebo turtlebot3_world.launch   

Ros package : https://github.com/ROBOTIS-GIT/turtlebot3_simulations 

Description: turtlebot3 robot models to simulate in gazebo and test slam and navigation packages. 

    Launch the SLAM eg. Gmapping to map the area/room and save the map.  

roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping 

    Launch the teleop node to move robot from key board. 

roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch 

( joystick also can be used, puspoe is to map the area and save this map )   

    Save the map after making full map of given room 

rosrun map_server map_saver -f ~/map  

    Launch the navigation node, to move the robot with path planning autonomously 

roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml 
