<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
<!-- code_chunk_output -->

* [git提交本地项目步骤](#git提交本地项目步骤)
* [md转HTML生成边栏目录](#md转html生成边栏目录httpsblogcsdnnetjackie_boboarticledetails79213988)

<!-- /code_chunk_output -->

# git提交本地项目步骤
1. 绑定用户
```sh {.line-numbers}
$ git config --global user.name "xxx"
$ git config --global user.email "xxx@xx.com"
```

2. 通过https上传
- 打开终端，进入本地项目文件夹
- 初始化.git文件，执行指令：`git init`
- 将所有文件添加到仓库，执行指令：`git add .`
- 提交文件，执行指令：`git commit -m "提交文件"`
- 关联github仓库，执行指令：`git remote add origin https://github.com/username/projectname.git`
- 上传本地代码，执行指令：`git push -u origin master`
- 可以通过如下命令进行代码合并[pull=fetch+merge]：`git pull --rebase origin master`

3. 输入用户名和密码，完成上传。

# [md转HTML生成边栏目录](https://blog.csdn.net/jackie_bobo/article/details/79213988)
安装：`npm install -g i5ting_toc`
执行指令：`i5ting_toc -f sample.md -o`
