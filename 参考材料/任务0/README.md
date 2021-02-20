### 检测git是否安装成功

在windows cmd任意路径下输入`git --version`，有出现`git version xxxxxxxxx`即说明安装成功

### 利用git提交本地文件至远程仓库

我们已经在https://github.com/NJUCS2021Spring 上为大家建好了各自的仓库，之后大家将要把自己的代码文件提交到上面的仓库中

首先大家在本地创建一个文件夹用于存放项目代码，例如这里我在D盘新建了文件夹`mycode`

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image.jfif)

打开cmd，进入mycode目录(在笔记本左下角快捷搜索cmd打开即可)

（第一行命令切换到D盘，第二行进入`mycode`，在C盘创建则无需切换到D）

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (1).jfif)

输入命令`git init`，在本地新建空仓库

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (2).jfif)

现在我们的`mycode`文件夹就相当于本地的空仓库了，我们需要设置远程仓库：输入命令`git remote add origin https://github.com/NJUCS2021Spring/xxx.git`(xxx为你的名字拼写，请大家先到https://github.com/NJUCS2021Spring 上确定自己的仓库名)

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (3).jfif)

现在我们设置好了远程仓库。之后我们会在本地仓库添加自己的文件、代码，并上传到远程仓库实现共享

##### 在本地仓库新建一个文件

在相应文件夹中新建一个文件，例如这里新建了文件`README.md`(鼠标右键“新建”)，在里面写点内容（如何编辑MarkDown格式的文件可见附录）

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (4).jfif)

我们可以通过命令`git status`查看上一次提交远程仓库后我们的本地仓库发生了什么变化：

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (5).jfif)

可以看到git提示我们之前还没有提交过，且本地仓库暂存区多出了还没有提交到远程仓库的文件`README.md`

##### 将本地文件提交到远程仓库

提交分为两个阶段，首先我们要将暂存区的本地文件上传至本地仓库：利用`git add`与`git commit`命令实现

输入命令`git add .`以添加所有新增的或者修改过的文件，再输入`git commit -m "first commit"`将添加的文件上传至本地仓库，并将本次提交的修改都加上注释“first commit”。`-m`选项后接的是代码修改注释，便于明确此次提交对代码做了哪些修改

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (6).jfif)

可以看到再次`git status`会提示所有变化都已经提交到本地仓库了

之后将本地仓库内容提交到远程仓库：

输入命令`git push -u origin main`，并根据提示输入自己的github账号和密码(密码输入时是不显示的)

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (7).jfif)

这里`git branch -M main`是为了修改本地分支的名字，`-M`选限后接新的分支名字；`git push -u origin main`中`-u`选项后接的`origin main`将当前已经提交的修改推送远程仓库的 main 分支下

这样提交后，我们就可以在https://github.com/NJUCS2021Spring 自己的仓库中看到我们提交的内容了



git是大家协同工作必备的工具，之后大二的ics、操作系统等课程也会使用到，感兴趣的同学可以进一步了解git的更多命令以及linux下的命令行，为后续学习做准备。这里附带一个教程链接https://www.liaoxuefeng.com/wiki/896043488029600



大家可以参考本文件向自己的仓库中添加写有自己名字的文件，熟悉git的使用

**注：上述所有命令够可以在Git Bash中执行**

​	Git Bash是Git for Windows 提供的一个仿真环境，可以从windows命令行执行git命令，在这个仿真环境下，使用git命令跟Linux 和 UNIX一样。同时该仿真环境内也可以执行Linux的一行原生命令。Windows端打开方式如下：

​	在资源管理器界面空白处点击鼠标右键，选中下图所示选项

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image.png)

​	出现下图所示窗口

![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (1).png)

​	在该窗口中同样可以按照前述流程敲入命令

![image-20210220134729351](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image-20210220134729351.png)



### 任务

​	为自己的仓库编写一个MarkDown格式的`README.md`文件，在文件中对自己的项目做一个介绍，内容包括但不限于以下：

+ **自己选择的项目**

+ **项目目标**

+ **项目功能（可适当细化）与实现情况**

  示例：

  ![](https://gitee.com/Coder-Colder/typora-pic-bed/raw/master/img/image (8).jfif)

### 附录

##### 如何编辑MarkDown文件？

1. 编辑器配置

   1. 推荐一款好用的MarkDown编辑器---Typora:https://typora.io/
   2. 或者使用：VSCode + MarkDown Extension

2. 快速学习MarkDown语法

   教程https://blog.csdn.net/zy440458/article/details/107778061

##### Git操作

教程https://www.liaoxuefeng.com/wiki/896043488029600





