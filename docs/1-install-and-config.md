# 1. Installing and Configuring Your ROS Environment

##  Checking that ROS was correctly installed

```bash
$ printenv | grep ROS
ROS_ETC_DIR=/opt/ros/melodic/etc/ros
ROS_ROOT=/opt/ros/melodic/share/ros
ROS_MASTER_URI=http://localhost:11311
ROS_VERSION=1
ROS_PYTHON_VERSION=2
ROS_PACKAGE_PATH=/opt/ros/melodic/share
ROSLISP_PACKAGE_DIRECTORIES=
ROS_DISTRO=melodic
```

## Create a ROS Workspace

- Create a Catkin workspace (showed paths were created within local folder structure)

```bash
$ mkdir -p ~/projects/master/1-integration/ros_tutorials/catkin_ws/src
$ cd ~/projects/master/1-integration/ros_tutorials/catkin_ws
$ catkin_make
...several output messages...
-- Build files have been written to: ~/projects/master/1-integration/ros_tutorials/catkin_ws/build
####
#### Running command: "make -j4 -l4" in "~/projects/master/1-integration/ros_tutorials/catkin_ws/build"
####
$
```

- Sourcing setup and checking

```bash
$ source devel/setup.bash
$ echo $ROS_PACKAGE_PATH
~/projects/master/1-integration/ros_tutorials/catkin_ws/src:/opt/ros/melodic/share
```
