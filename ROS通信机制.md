ros吸引人的地方两个，一、有各种现成的解决领域问题的软件包，二、有一个现成的构建分布并发系统软件的方案，既通信中间件。

master提供两种基础服务，naming service和parameter server。这两个服务本质上没有什么不同，就是注册和查询，只不过一个是地址，一个是参数。这些是远远不够的。动态发现discovery，生存检测liveness，访问控制access control，这些基本的都没有。
