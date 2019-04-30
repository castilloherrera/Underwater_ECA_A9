# Underwater_ECA_A9
# Installation 

--> Copy the files in your Workspace 

cd ~/name_of_workspace

git clone https://github.com/castilloherrera/Underwater_ECA_A9.git

--> Then build your workspace using 

    Whit the Simulator Underwater 
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

and then 

    roslaunch gazebo_und start_underwater.launch
