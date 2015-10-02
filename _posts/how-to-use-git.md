title: Hey，let us git ！
date: 2015-09-22 12:30:16
categories: skill
tags: git
---
程序员の日常：

┋◆冃.狌.交.伖，释.鲂.压.劦、棑.解.漃.瘼◆ 真 人】视||频. █网.址：wWw. GitHub .Com◆┋
![](http://i1.tietuku.com/cfbad19f8d74fd71.jpg)



github刷的飞起，git怎能只一知半解，花了一上午时间撸完了[史上最浅显易懂的Git教程](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)，不得不说廖大大写的教程炒鸡棒，包括之前的python教程：）然后总结了一下git常用的指令如下：

----------


# 创建版本库 #
初始化一个Git仓库，使用`git init`命令。

添加文件到Git仓库，分两步：

- 第一步，使用命令`git add <file>`，注意，可反复多次使用，添加多个文件；

- 第二步，使用命令`git commit`，完成。

----------
# 版本控制 #

要随时掌握工作区的状态，使用`git status`命令。

如果`git status`告诉你有文件被修改过，用`git diff`可以查看修改内容。


----------
# 工作区和暂存区
![](http://i13.tietuku.com/0b2d71ab51b7e2b6.jpg)

现在，你又理解了Git是如何跟踪修改的，每次修改，如果不add到暂存区，那就不会加入到commit中。

----------
# 添加远程库 #

- 要关联一个远程库，使用命令`git remote add origin git@server-name:path/repo-name.git`；

- 关联后，使用命令`git push -u origin master`第一次推送master分支的所有内容；

- 此后，每次本地提交后，只要有必要，就可以使用命令`git push origin master`推送最新修改；

分布式版本系统的最大好处之一是在本地工作完全不需要考虑远程库的存在，也就是有没有联网都可以正常工作，而SVN在没有联网的时候是拒绝干活的！当有网络的时候，再把本地提交推送一下就完成了同步，真是太方便了！

----------
# 从远程克隆 #
要克隆一个仓库，首先必须知道仓库的地址，然后使用`git clone`命令克隆。
 
    $ git clone git@github.com:feidapeng/helloworld.git


Git支持多种协议，包括https，但通过ssh支持的原生git协议速度最快。

----------
# 多人协作 #
多人协作的工作模式通常是这样：

- 首先，可以试图用`git push origin branch-name`推送自己的修改；

- 如果推送失败，则因为远程分支比你的本地更新，需要先用`git pull`试图合并；

- 如果合并有冲突，则解决冲突，并在本地提交；

- 没有冲突或者解决掉冲突后，再用`git push origin branch-name`推送就能成功！

如果`git pull`提示“no tracking information”，则说明本地分支和远程分支的链接关系没有创建，用命令

    git branch --set-upstream branch-name origin/branch-name
查看远程库信息，使用`git remote -v`；


在本地创建和远程分支对应的分支，使用`GIT CHECKOUT -B BRANCH-NAME ORIGIN/BRANCH-NAME`，本地和远程分支的名称最好一致.  


  

> 祝同性交友愉快