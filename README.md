# Underwater_ECA_A9
# Installation 

--> Copy the files in your Workspace 

cd ~/name_of_workspace

git clone https://github.com/castilloherrera/Underwater_ECA_A9.git

--> Then build your workspace using 

     **** Whit the Simulator Underwater 
     **** git clone https://github.com/castilloherrera/Simulator_Underwater.git
     
cd ~/catkin_ws

catkin_make install

or

cd ~/catkin_ws

catkin build

(in case you are using catkin_tools.)


# Start

Start an empty underwater environment using either

roslaunch worlds ocean_waves.launch
