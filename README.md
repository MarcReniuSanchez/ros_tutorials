# ROS tutorials

## Installation

Followed instructions and environment configuration in http://wiki.ros.org/melodic/Installation/Ubuntu.

Commands executed listed in
[Installation](https://github.com/MarcReniuSanchez/ros_tutorials/tree/master/docs/0-installation.md) docs.

## 1. Installing and Configuring Your ROS Environment

Followed tutorial for [Installing and Configuring Your ROS Environment](http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment).

Commands executed listed in
[Installing and Configuring Your ROS Environment](https://github.com/MarcReniuSanchez/ros_tutorials/tree/master/docs/1-install-and-config.md) docs.

## 2. Navigating the ROS Filesystem

Followed tutorial for [Navigating the ROS Filesystem](http://wiki.ros.org/ROS/Tutorials/NavigatingTheFilesystem).

Understanding the `ros<pack find | cd | ls> [package name]` commands.

## 3. Creating a ROS Package

Followed tutorial for [Creating a ROS Package](http://wiki.ros.org/ROS/Tutorials/CreatingPackage).

Created a new `beginner_tutorial` package. Filling `/src/beginner_tutorials/package.xml` with some custom information and removed all commented lines.

## 4. Building Packages

Followed tutorial for [Building Packages](http://wiki.ros.org/ROS/Tutorials/BuildingPackages).

Readed and be sure that `/build` and `/devel` folder were created locally. `.gitignore` file is configured to ignore this folder to be pushed up to the repository.

## 5. Understanding ROS Nodes

Followed tutorial for [Understanding ROS Nodes](http://wiki.ros.org/ROS/Tutorials/UnderstandingNodes).

ROS commands executions listed in [Understanding ROS Nodes](https://github.com/MarcReniuSanchez/ros_tutorials/tree/master/docs/5-ros-nodes.md) docs.

## 6. Understanding ROS Topics

Followed tutorial for [Understanding ROS Topics](http://wiki.ros.org/ROS/Tutorials/UnderstandingTopics).

Playing with `turtlesim`, and using `rqt_graph`, `rostopic`, `rosmsg`, and `rqt_plot` to see how they work.

## 7. Understanding ROS Services and Parameters

Followed tutorial for [Understanding ROS Services and Parameters](http://wiki.ros.org/ROS/Tutorials/UnderstandingServicesParams).

Using `rosservice` and `rosparams` to manipulate and understant services and parameters in ROS.

## 8. Using rqt_console and roslaunch

Only readed

## 9. Using rosed to edit files in ROS

Only readed

## 10. Creating a ROS msg and srv

Followed tutorial for [Creating a ROS msg and srv](http://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv).

Created `msg/Num.msg` a `srv/AddTwoInts.srv` files as explained in tutorials, compiled and installed.
Only issue found was creating the message file outside `msg` folder by mistake.
