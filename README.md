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
