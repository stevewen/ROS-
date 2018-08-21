<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->

* [ROS学习笔记](#ros学习笔记)
	* [编译ROS工作空间中的某一个包](#编译ros工作空间中的某一个包)
	* [catkin_make](#catkin_make)

<!-- /code_chunk_output -->

# ROS学习笔记
## 编译ROS工作空间中的某一个包
`$ catkin_make -DCATKIN_WHITELIST_PACKAGES="package1;package2"`
[详细请查看：catkin_make](http://wiki.ros.org/catkin/commands/catkin_make)

## catkin_make
1.  不依赖的单独编译工作空间中的各个程序包：使用catkin_make_isolated，如果你的两个程序包包含了两个相同名称的节点，而你不使用该命令进行编译的话，则会出现依赖错误。
2. 如果程序包的源文件不在当前工作空间中，可以使用：catkin_make –source xx文件所在路径。
