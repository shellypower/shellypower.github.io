---
layout:     post
title:      "如何搭建个人博客"
subtitle:   "我的第一篇技术分享，也不知道记了些啥"
date:       2017-07-08
author:     "Shelly"
header-img: "img/post-bg-os-metro.jpg"
catalog: true
tags:
    - 前端开发
    - Jekyll
 
    
---


# 搭建个人博客

---

在这里介绍的是如何用jekyll搭建自己的个人博客,首先你得在linux系统上安装几个必要的插件，以便安装jekyll.

### 安装Ruby和RubyGems

sudo apt-get install ruby  //在深度终端输入这条命令

### 安装yum

sudo apt-get install yum
<br>sudo yum install ruby-dev/sudo yum install ruby-devel

 > "没有已启用的仓库。
  执行 "yum repolist all" 查看您拥有的仓库。
  您可以用 yum-config-manager --enable &lt;仓库名&gt;          来启用仓库"

sudo apt-get install ruby-dev //建仓库

### 安装Jekyll

sudo gem install jekyll
>ERROR:  Error installing jekyll:
	invalid gem: package is corrupt, exception while verifying: undefined method `size' for nil:NilClass (NoMethodError) in /var/lib/gems/2.3.0/cache/ffi-1.9.18.gem
	
<br>需删除gem目录下的cache文件夹
<br>cd /var/lib/gems/2.3.0/
<br>$sudo rm -rf cache
<br>sudo gem install jekyll
<br>sudo gem install bundler

### 创建本地网页

<br>jekyll new my-awesome-site
<br>cd my-awesome-site
<br>jekyll build//建立
<br>jekyll serve//运行

### 使用下载的模板

<br>解压后将模板内的文件复制到 my-awesome-site 文件夹
<br>jekyll build//建立 
<br>jekyll serve//运行

### 带有YAML头信息的markdown文件

<br>layout: post
<br>title: 这里是题目
<br>tags:
- 标签1
- 标签2
<br>categories: 分类
<br>description: 描述。

<br>push到github,就能渲染成html 如何下载和使用模板

### 建立仓库

<br>echo "# shelly" >> README.md
<br>git init
<br>git add README.md
<br>git commit -m "first commit"
<br>git remote add origin https://github.com/shellypower/shelly.git
<br>git push -u origin master

### push an existing repository from the command line

<br>git remote add origin https://github.com/shellypower/shellypower.github.io
<br>git remote rm origin
<br>git remote add origin https://github.com/shellypower/shellypower.github.io
<br>git push -u origin master

### 提示出错信息：fatal: remote origin already exists.

   > 解决办法如下： 
    1、先输入$ git remote rm origin
    2、再输入$ git remote add origin git@github.com:djqiang/gitdemo.git 就不会报错了！

