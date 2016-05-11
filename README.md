vrep_youbot_plugin
==================

Installation
--

1) Install youBot ROS packages e.g.  
```
$ sudo apt-get install ros-indigo-youbot-driver-ros-interface
```
2) Install v-rep (http://www.v-rep.eu/) into i.e. /opt/v-rep

3) Clone the repository into your catkin workspace

4) Copy vrep_common and vrep_plugin ros packages to your catkin workspace (same workspace where you put this package)

    $ cp -r [VREP FOLDER]/programming/ros_packages/vrep_plugin ~/catkin_ws/src/
    $ cp -r [VREP FOLDER]/programming/ros_packages/vrep_common ~/catkin_ws/src/

5) Compile

    $ catkin_make

6) Copy the compiled libraries libv_repExtyouBot.so and libv_repExtRos.so into your /opt/v-rep directory

    $ sudo cp ~/catkin_ws/devel/lib/libv_repExt* [VREP FOLDER]

* Replace each occurrence of [VREP FOLDER] with your vrep installation full path

