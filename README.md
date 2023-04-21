# sms-midterm
'''
ubuntu2005@ubuntu:~$ ls
assigment3_ws   assignment4     Downloads              Pictures     Public        week3
assignment_1    assignment4_ws  install_ros_noetic.sh  project2     sms-project3  week3.sh
assignment2     catkin_ws       midterm                project2+ws  SMS-WS        week3.sh.save
assignment2_ws  Desktop         midterm_ws             project2_ws  Templates
assignment3_ws  Documents       Music                  project4_ws  Videos
ubuntu2005@ubuntu:~$ cd catkin_ws/
ubuntu2005@ubuntu:~/catkin_ws$ mkdir midterm
mkdir: cannot create directory ‘midterm’: File exists
ubuntu2005@ubuntu:~/catkin_ws$ mkdir src
mkdir: cannot create directory ‘src’: File exists
ubuntu2005@ubuntu:~/catkin_ws$ cd src
ubuntu2005@ubuntu:~/catkin_ws/src$ catkin_create_pkg midterm roscpp
usage: catkin_create_pkg [-h] [--meta] [-s [SYS_DEPS [SYS_DEPS ...]]]
                         [-b [BOOST_COMPS [BOOST_COMPS ...]]] [-V PKG_VERSION] [-D DESCRIPTION]
                         [-l LICENSE] [-a AUTHOR] [-m MAINTAINER] [--rosdistro ROSDISTRO]
                         name [dependencies [dependencies ...]]
catkin_create_pkg: error: File exists: /home/ubuntu2005/catkin_ws/src/midterm/package.xml
ubuntu2005@ubuntu:~/catkin_ws/src$ mkdir launch
ubuntu2005@ubuntu:~/catkin_ws/src$ cd ..
ubuntu2005@ubuntu:~/catkin_ws$ catkin_make
Base path: /home/ubuntu2005/catkin_ws
Source space: /home/ubuntu2005/catkin_ws/src
Build space: /home/ubuntu2005/catkin_ws/build
Devel space: /home/ubuntu2005/catkin_ws/devel
Install space: /home/ubuntu2005/catkin_ws/install
####
#### Running command: "cmake /home/ubuntu2005/catkin_ws/src -DCATKIN_DEVEL_PREFIX=/home/ubuntu2005/catkin_ws/devel -DCMAKE_INSTALL_PREFIX=/home/ubuntu2005/catkin_ws/install -G Unix Makefiles" in "/home/ubuntu2005/catkin_ws/build"
####
-- Using CATKIN_DEVEL_PREFIX: /home/ubuntu2005/catkin_ws/devel
-- Using CMAKE_PREFIX_PATH: /opt/ros/noetic
-- This workspace overlays: /opt/ros/noetic
-- Found PythonInterp: /usr/bin/python3 (found suitable version "3.8.10", minimum required is "3") 
-- Using PYTHON_EXECUTABLE: /usr/bin/python3
-- Using Debian Python package layout
-- Using empy: /usr/lib/python3/dist-packages/em.py
-- Using CATKIN_ENABLE_TESTING: ON
-- Call enable_testing()
-- Using CATKIN_TEST_RESULTS_DIR: /home/ubuntu2005/catkin_ws/build/test_results
-- Forcing gtest/gmock from source, though one was otherwise available.
-- Found gtest sources under '/usr/src/googletest': gtests will be built
-- Found gmock sources under '/usr/src/googletest': gmock will be built
-- Found PythonInterp: /usr/bin/python3 (found version "3.8.10") 
-- Using Python nosetests: /usr/bin/nosetests3
-- catkin 0.8.10
-- BUILD_SHARED_LIBS is on
-- BUILD_SHARED_LIBS is on
-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-- ~~  traversing 1 packages in topological order:
-- ~~  - midterm
-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-- +++ processing catkin package: 'midterm'
-- ==> add_subdirectory(midterm)
-- Configuring done
-- Generating done
-- Build files have been written to: /home/ubuntu2005/catkin_ws/build
####
#### Running command: "make -j2 -l2" in "/home/ubuntu2005/catkin_ws/build"
####
ubuntu2005@ubuntu:~/catkin_ws$ mkdir midterm
mkdir: cannot create directory ‘midterm’: File exists
ubuntu2005@ubuntu:~/catkin_ws$ cd midterm
ubuntu2005@ubuntu:~/catkin_ws/midterm$ git clone "https://github.com/Izzatullokh24/sms-midterm.git"
Cloning into 'sms-midterm'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 600 bytes | 600.00 KiB/s, done.
ubuntu2005@ubuntu:~/catkin_ws/midterm$ catkin_make
Base path: /home/ubuntu2005/catkin_ws/midterm
Source space: /home/ubuntu2005/catkin_ws/midterm/src
Build space: /home/ubuntu2005/catkin_ws/midterm/build
Devel space: /home/ubuntu2005/catkin_ws/midterm/devel
Install space: /home/ubuntu2005/catkin_ws/midterm/install
####
#### Running command: "make cmake_check_build_system" in "/home/ubuntu2005/catkin_ws/midterm/build"
####
####
#### Running command: "make -j2 -l2" in "/home/ubuntu2005/catkin_ws/midterm/build"
####
ubuntu2005@ubuntu:~/catkin_ws/midterm$ 
'''

ubuntu2005@ubuntu:~/catkin_ws/midterm$ roscore
... logging to /home/ubuntu2005/.ros/log/5be03362-e04a-11ed-af3b-8dc38783555c/roslaunch-ubuntu-8450.log
Checking log directory for disk usage. This may take a while.
Press Ctrl-C to interrupt
Done checking log file disk usage. Usage is <1GB.

started roslaunch server http://ubuntu:37759/
ros_comm version 1.16.0


SUMMARY
========

PARAMETERS
 * /rosdistro: noetic
 * /rosversion: 1.16.0

NODES

auto-starting new master
process[master]: started with pid [8458]
ROS_MASTER_URI=http://ubuntu:11311/

setting /run_id to 5be03362-e04a-11ed-af3b-8dc38783555c
process[rosout-1]: started with pid [8468]
started core service [/rosout]






ubuntu2005@ubuntu:~/catkin_ws/midterm$ source devel/setup.bash 
ubuntu2005@ubuntu:~/catkin_ws/midterm$ rossrv list
control_msgs/QueryCalibrationState
control_msgs/QueryTrajectoryState
control_toolbox/SetPidGains
controller_manager_msgs/ListControllerTypes
controller_manager_msgs/ListControllers
controller_manager_msgs/LoadController
controller_manager_msgs/ReloadControllerLibraries
controller_manager_msgs/SwitchController
controller_manager_msgs/UnloadController
diagnostic_msgs/AddDiagnostics
diagnostic_msgs/SelfTest
dynamic_reconfigure/Reconfigure
gazebo_msgs/ApplyBodyWrench
gazebo_msgs/ApplyJointEffort
gazebo_msgs/BodyRequest
gazebo_msgs/DeleteLight
gazebo_msgs/DeleteModel
gazebo_msgs/GetJointProperties
gazebo_msgs/GetLightProperties
gazebo_msgs/GetLinkProperties
gazebo_msgs/GetLinkState
gazebo_msgs/GetModelProperties
gazebo_msgs/GetModelState
gazebo_msgs/GetPhysicsProperties
gazebo_msgs/GetWorldProperties
gazebo_msgs/JointRequest
gazebo_msgs/SetJointProperties
gazebo_msgs/SetJointTrajectory
gazebo_msgs/SetLightProperties
gazebo_msgs/SetLinkProperties
gazebo_msgs/SetLinkState
gazebo_msgs/SetModelConfiguration
gazebo_msgs/SetModelState
gazebo_msgs/SetPhysicsProperties
gazebo_msgs/SpawnModel
laser_assembler/AssembleScans
laser_assembler/AssembleScans2
map_msgs/GetMapROI
map_msgs/GetPointMap
map_msgs/GetPointMapROI
map_msgs/ProjectedMapsInfo
map_msgs/SaveMap
map_msgs/SetMapProjections
nav_msgs/GetMap
nav_msgs/GetPlan
nav_msgs/LoadMap
nav_msgs/SetMap
nodelet/NodeletList
nodelet/NodeletLoad
nodelet/NodeletUnload
pcl_msgs/UpdateFilename
polled_camera/GetPolledImage
roscpp/Empty
roscpp/GetLoggers
roscpp/SetLoggerLevel
roscpp_tutorials/TwoInts
rospy_tutorials/AddTwoInts
rospy_tutorials/BadTwoInts
rviz/SendFilePath
sensor_msgs/SetCameraInfo
std_srvs/Empty
std_srvs/SetBool
std_srvs/Trigger
tf/FrameGraph
tf2_msgs/FrameGraph
topic_tools/DemuxAdd
topic_tools/DemuxDelete
topic_tools/DemuxList
topic_tools/DemuxSelect
topic_tools/MuxAdd
topic_tools/MuxDelete
topic_tools/MuxList
topic_tools/MuxSelect
turtlesim/Kill
turtlesim/SetPen
turtlesim/Spawn
turtlesim/TeleportAbsolute
turtlesim/TeleportRelative
ubuntu2005@ubuntu:~/catkin_ws/midterm$ rosrun midterm service_server
[rosrun] Couldn't find executable named service_server below /home/ubuntu2005/catkin_ws/midterm/src/midterm
ubuntu2005@ubuntu:~/catkin_ws/midterm$ 





ubuntu2005@ubuntu:~/catkin_ws/midterm$ source devel/setup.bash
ubuntu2005@ubuntu:~/catkin_ws/midterm$ rosservice list
/rosout/get_loggers
/rosout/set_logger_level
ubuntu2005@ubuntu:~/catkin_ws/midterm$ rosservice call /weather_station Istanbul
ERROR: Service [/weather_station] is not available.
ubuntu2005@ubuntu:~/catkin_ws/midterm$ 

ubuntu2005@ubuntu:~/catkin_ws/midterm$ source devel/setup.bash
ubuntu2005@ubuntu:~/catkin_ws/midterm$ roslaunch midterm speed_check_simulator.launch
RLException: [speed_check_simulator.launch] is neither a launch file in package [midterm] nor is [midterm] a launch file name
The traceback for the exception was written to the log file
ubuntu2005@ubuntu:~/catkin_ws/midterm$ rosparam list
/rosdistro
/roslaunch/uris/host_ubuntu__37759
/rosversion
/run_id
ubuntu2005@ubuntu:~/catkin_ws/midterm$ osparam dump

Command 'osparam' not found, did you mean:

  command 'ohparam' from deb openhpi-clients (3.8.0-2build4)
  command 'rosparam' from deb python3-rosparam (1.14.3+ds1-11ubuntu5)

Try: sudo apt install <deb name>

ubuntu2005@ubuntu:~/catkin_ws/midterm$ rosparam dump
rosdistro: 'noetic

  '
roslaunch:
  uris:
    host_ubuntu__37759: http://ubuntu:37759/
rosversion: '1.16.0

  '
run_id: 5be03362-e04a-11ed-af3b-8dc38783555c
ubuntu2005@ubuntu:~/catkin_ws/midterm$ rostopic echo speed
WARNING: topic [/speed] does not appear to be published yet
rosparam set speed 68








  



