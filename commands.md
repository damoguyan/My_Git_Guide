安装配置
=====================
(1)名称 公开仓库时给别人看的
$git config --global user.name "yourname"  //注意可以使用昵称以保护隐私
$git  config --global user.email "your_email@XX.com"
(2) 可以让命令输出拥有更高的可读性
$git config --global color.ui auto
(3)
以上配置均保存在~/.gitconfig文件中，所以也可以直接创建或修改这个文件

概念解释
===========================
工作区（Working Directory----电脑里看到目录，比如test：
版本库（Repository）-工作区有一个隐藏目录.git，这个不算工作区，而是Git的版本库
版本库最重要的3个东西：
(1)暂存区stage（或者叫index）
(2)自动创建的第一个分支'master'
(3)指向master的一个指针'HEAD'
提交流程： 工作区文件--->暂存区(add命令实现)---->加入master(通过commit命令实现)



======================
$mkdir test #工作区
$cd test 
$git init   #版本库

常用命令 
===================
$git  add file1 file2
$git  commit -m "message"
$git  status          #仓库当前的状态
$git  diff
$git  log
$git checkout -- file  #没有--，就变成了“切换到另一个分支”的命令


版本跳转
==============
回到过去
-----------
$git log
$git reset --hard commit_id   #(git的版本号不是1,2,3而是hash值，输入可以区分版本的前几位即可)
$git reset --hard  HEAD   #HEAD表示当前版本 （HEAD^  HEAD^^  HEAD~10）分别表示当前版本的前一个，2个 10个版本
去曾经到达的未来
-----------------
$git reflog   #查看命令历史 主要是为了看commit_id
$git reset --hard commit_id 

删除文件
=================
(1)先本地工作区删除
$rm test.md
(2)确实要删除版本库的文件
$git rm test.rm
(3)删错了
$git checkout -- test.md


远程仓库
==============
推送到远程(github)
---------------------
(1)第一次$ ssh-keygen -t rsa -C "youremail@example.com"  #将生成的公钥Key添加到自己github账户的ssh设置中
(2)在github网站上创建repository，名字如My_Git_Guide
(3)根据网站提示在自己电脑上分别运行下面命令
$git remote add origin https://github.com/damoguyan/My_Git_Guide.git #把一个已有的本地仓库与之关联
$git push -u origin master  #把当前分支master推送到远程 第一次加-u
(4)后续本地有改动，推送到远程
$git push origin master

从远程clone
--------------------
$git clone git@github.com:damoguyan/bitcoinbook.git #Git支持多种协议，包括https，但通过ssh支持的原生git协议速度最快


