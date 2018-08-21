# git提交本地项目步骤
1.绑定用户
```
$ git config --global user.name "xxx"
$ git config --global user.email "xxx@xx.com"
```
2.通过https上传
- 打开终端，进入本地项目文件夹
- 初始化.git文件，执行指令：`git init`
- 将所有文件添加到仓库，执行指令：`git add .`
- 提交文件，执行指令：`git commit -m "提交文件"`
- 关联github仓库，执行指令：`git remote add origin https://github.com/username/projectname.git`
- 上传本地代码，执行指令：`git push -u origin master`
- 可以通过如下命令进行代码合并[pull=fetch+merge]:`git pull --rebase origin master`
