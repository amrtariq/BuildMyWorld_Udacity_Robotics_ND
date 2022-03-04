# Build_My_World_Udacity_Robotics_ND

![image](https://user-images.githubusercontent.com/18179768/156837970-6ba5d786-988d-4fcb-a590-aa59ca3af81f.png)

The Target was to build simple world in Model Editor tool & Building Editor tool in Gazebo and add a Gazebo Plugin to print constant message when it runs.
## Structure

.Project1                          # Build My World Project 
    ├── model                          # Model files 
    │   ├── Building
    │   │   ├── model.config
    │   │   ├── model.sdf
    │   ├── Humanoid
    │   │   ├── model.config
    │   │   ├── model.sdf
    |   ├── two_wheel
    │   │   ├── model.config
    │   │   ├── model.sdf
    ├── script                         # Gazebo World plugin C++ script      
    │   ├── hello.cpp
    ├── world                          # Gazebo main World containing models 
    │   ├── myworld.world
    ├── CMakeLists.txt                 # Link libraries 
    └──                              

## Clone and Build
Step 1: Create new catkin_ws

Step 2: Clone into your new package into your ws folder

Step 3 : Create a build directory and compile the code

$ cd ~/workspace/package/
$ catkin_make

Step 4 : Add the library path to the Gazebo plugin path

$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:~/package/build

Step 4: run 

$ gazebo myworld.world
