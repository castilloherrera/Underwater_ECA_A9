# Underwater_ECA_A9
# Installation 

Copy the files in your Workspace 

cd ~/name_of_workspace

    git clone https://github.com/castilloherrera/Underwater_ECA_A9.git

Then, build your workspace using 

    With the Simulator Underwater 
    git clone https://github.com/castilloherrera/Simulator_Underwater.git
     
cd ~/catkin_ws

catkin_make install

or

cd ~/catkin_ws

catkin build

(in case you are using catkin_tools.)


# Start

To run a demosntration with the underwater, you can run a Simulator Underwater scenario, such as

    roslaunch worlds ocean_waves.launch

and then: 

 -For a circular trajectory :
 
    roslaunch gazebo_und start_trajectory_control_circle.launch
    
 -For a rectangle trajectory :

    roslaunch gazebo_und start_trajectory_control_rectangle.launch
    
 -For a underwater fleet :

    roslaunch gazebo_und start_underwater_fleet.launch
  
  WARNING: 
  
 By default the simulation of underwater fleet, starts with 4 underwater for change this option :
  
   -If you want 20 underwaters (go to -> /gazebo_und/launch/start_underwater_fleet.launch) :
   
   uncomment :
   
    <node name="rviz" pkg="rviz" type="rviz" output="screen" args="-d $(find control)/rviz/eca_a9_control_fleet_20.rviz"/>
     
   and comment :
   
     <node name="rviz" pkg="rviz" type="rviz" output="screen" args="-d $(find control)/rviz/eca_a9_control_fleet_4.rviz"/>
    
   Then, go to -> /gazebo_und/launch/underwater_fleet/ten_underwater_row.launch and uncomment all the underwaters.
    
     
   -If you want 10 underwaters (go to -> /gazebo_und/launch/start_underwater_fleet.launch) :
   
   uncomment :
   
    <node name="rviz" pkg="rviz" type="rviz" output="screen" args="-d $(find control)/rviz/eca_a9_control_fleet_10.rviz"/>
 
   and comment:
     
     <node name="rviz" pkg="rviz" type="rviz" output="screen" args="-d $(find control)/rviz/eca_a9_control_fleet_4.rviz"/>
     
   Then, go to -> /gazebo_und/launch/underwater_fleet/ten_underwater_row.launch and uncomment the next 3 underwaters.
     
  
  
