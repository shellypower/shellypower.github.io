---
layout:     post
title:      " 常用的深度终端命令行 "
subtitle:   " 深度是一个好用的系统，后台命令行控制也很方便 "
date:       2017-07-1 12:00:00
author:     "Shelly"
header-img: "img/post-bg-alibaba.jpg"
tags:
    - 深度学习
    
---

# 深度终端命令行

 linxus

---

深度终端命令行
安装软件包Sudo apt-get install atom
卸载软件sudo apt-get remove ruby
打开软件 atom .
进入文件 cd des+Tap 补齐
查看所在位置 pwd
创建文件夹 mkdir+文件夹名
创建文件 vim file（文件名）
删除文件 rm file
删除文件夹 rm -r dir
移动文件到dir  mv file dir
清屏 Ctrl l
重命名 mv file1 file2
复制 cp file1 file3 /   cp -r dir dir1
查看文件类型 file file2
查看文件 cat file2
以管理员身份执行操作 sudo
普通用户切换为管理员用户 sudo su
查看ruby版本号  ruby -v
找到ruby的位置 whereis ruby
退出编辑：wq

建立仓库
echo "# dapengyou.github.com" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/dapengyou/dapengyou.github.com.git
git push -u origin master

###建立仓库
echo "# shelly" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/shellypower/shelly.git
git push -u origin master
###push an existing repository from the command line
git remote add origin https://github.com/shellypower/shellypower.github.io
git remote rm origin
git remote add origin https://github.com/shellypower/shellypower.github.io
git push -u origin master
###提示出错信息：fatal: remote origin already exists.
    解决办法如下：
    1、先输入$ git remote rm origin
    2、再输入$ git remote add origin git@github.com:djqiang/gitdemo.git 就不会报错了！
