# Understanding ROS Nodes

- Initializing `roscore`

```bash
$ roscore
... logging to ~/.ros/log/55452d82-dc99-11e8-bbab-48d2243fbef3/roslaunch-marc-toshi-9707.log
Checking log directory for disk usage. This may take awhile.
Press Ctrl-C to interrupt
Done checking log file disk usage. Usage is <1GB.

started roslaunch server http://marc-toshi:42033/
ros_comm version 1.14.3


SUMMARY
========

PARAMETERS
 * /rosdistro: melodic
 * /rosversion: 1.14.3

NODES

auto-starting new master
process[master]: started with pid [9718]
ROS_MASTER_URI=http://marc-toshi:11311/

setting /run_id to 55452d82-dc99-11e8-bbab-48d2243fbef3
process[rosout-1]: started with pid [9729]
started core service [/rosout]
```

- Checkink `rosnode` and info of `roscore`

```bash
$ rosnode list
/rosout
$ rosnode info /rosout
--------------------------------------------------------------------------------
Node [/rosout]
Publications:
 * /rosout_agg [rosgraph_msgs/Log]

Subscriptions:
 * /rosout [unknown type]

Services:
 * /rosout/get_loggers
 * /rosout/set_logger_level


contacting node http://marc-toshi:41469/ ...
Pid: 9729
```

- Starting `turtlesim` node

```bash
$ rosrun turtlesim turtlesim_node
[ INFO] [1540941309.555352090]: Starting turtlesim with node name /turtlesim
[ INFO] [1540941309.566031750]: Spawning turtle [turtle1] at x=[5,544445], y=[5,544445], theta=[0,000000]
$ rosrun turtlesim turtlesim_node __name:=my_turtle
[ INFO] [1540941478.895064203]: Starting turtlesim with node name /my_turtle
[ INFO] [1540941478.905309283]: Spawning turtle [turtle1] at x=[5,544445], y=[5,544445], theta=[0,000000]
```

- Checking `rosnode` info

```bash
$ rosnode list
/rosout
/turtlesim
$ rosnode list
/my_turtle
/rosout
$ rosnode ping my_turtle
rosnode: node is [/my_turtle]
pinging /my_turtle with a timeout of 3.0s
xmlrpc reply from http://marc-toshi:34769/	time=0.770092ms
xmlrpc reply from http://marc-toshi:34769/	time=1.013041ms
xmlrpc reply from http://marc-toshi:34769/	time=1.255035ms
xmlrpc reply from http://marc-toshi:34769/	time=1.291990ms
xmlrpc reply from http://marc-toshi:34769/	time=1.384020ms
[stoping...]ping average: 1.142836ms
```

- Checking `rosnode` after stoping `master` execution

```bash
$ rosnode list
ERROR: Unable to communicate with master!
```
