安装
=====================
$git config --global user.name "yourname"
$git  config --global user.email "your_email@XX.com"


创建仓库(repository)
======================
$mkdir test
$cd test 
$git init

常用命令 
===================
$git  add file1 file2
$git  commit -m "message"
$git  status          #仓库当前的状态
$git  diff
$git  log


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
