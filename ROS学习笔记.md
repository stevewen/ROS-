<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

* [ROS学习笔记](#ros学习笔记)
	* [编译ROS工作空间中的某一个包](#编译ros工作空间中的某一个包)
	* [catkin_make 相关](#catkin_make-相关)
	* [Matlab-ROS 联合控制](#matlab-ros-联合控制)

<!-- /code_chunk_output -->

# ROS学习笔记

## 编译ROS工作空间中的某一个包

`$ catkin_make -DCATKIN_WHITELIST_PACKAGES="package1;package2"`
[详细请查看：catkin_make](http://wiki.ros.org/catkin/commands/catkin_make)

## catkin_make 相关

1.  不依赖的单独编译工作空间中的各个程序包：使用catkin_make_isolated，如果你的两个程序包包含了两个相同名称的节点，而你不使用该命令进行编译的话，则会出现依赖错误。
2.  如果程序包的源文件不在当前工作空间中，可以使用：catkin_make –source xx文件所在路径。


## Matlab-ROS 联合控制

1. 在ROS中
- 开启ROS主节点 `roscore`
- 启动turtlebot节点 `rosrun turtlesim turtlesim_node`

2. 在MATLAB中
- 初始化ROS环境 `rosinit()`
- 查看ROS话题 `rostopic list`
- 运行 random_turtle_realtime.slx


## moveit配置三维环境
