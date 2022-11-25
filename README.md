**This readme is to install and get to know about the gazebo(ignition) and how it works with ROS2**

Prerequistes:
* Install Ros2 
* Install ignition version Fortress

[Follow this to install Ros and gazebo(ignition)](https://docs.ros.org/en/humble/Tutorials/Advanced/Simulators/Gazebo.html)

Gazebo vs Ignition:

The Gazebo that we all know from before is not going to be supported anymore
The another simulation software called ignition has been in development for a long time in parallel with gazebo 
Now the ignition got popular and it is more advance than classic gazebo, The Open source robotics foundation is renaming  the ignition software as gazebo
and dropping the development of classical gazebo

From Gazebo Garden both Gazebo and ignition are same 

**NOTE:**
  * Ignition have a separate environment and the topics available inside the ignition environment cannot be accesed outside by ROS2.
  * [ros_gz_bridge](https://github.com/gazebosim/ros_gz/blob/humble/ros_gz_bridge/README.md) is a library that supports the transportation of topics from ignition --> ROS2 or viceverca or bidirectional


**To bridge a topic bidirectionally:**

    $ ros2 run ros_gz_bridge parameter_bridge /<topic_name>@<ROS2-msg-type>@<ignition-msg-type>


