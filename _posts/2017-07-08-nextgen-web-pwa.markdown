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

##安装Ruby和RubyGems
sudo apt-get install ruby

###安装yum
sudo apt-get install yum
sudo yum install ruby-dev/sudo yum install ruby-devel

 > "没有已启用的仓库。
  执行 "yum repolist all" 查看您拥有的仓库。
  您可以用 yum-config-manager --enable &lt;仓库名&gt;          来启用仓库"

sudo apt-get install ruby-dev //建仓库
##安装Jekyll
sudo gem install jekyll
>ERROR:  Error installing jekyll:
	invalid gem: package is corrupt, exception while verifying: undefined method `size' for nil:NilClass (NoMethodError) in /var/lib/gems/2.3.0/cache/ffi-1.9.18.gem
	
需删除gem目录下的cache文件夹
cd /var/lib/gems/2.3.0/
$sudo rm -rf cache
sudo gem install jekyll
sudo gem install bundler
##创建本地网页
 jekyll new my-awesome-site
cd my-awesome-site
jekyll build//建立
 jekyll serve//运行

##如何下载和使用模板
下载模板
解压后将模板内的文件复制到 my-awesome-site 文件夹
jekyll build//建立 
jekyll serve//运行
###带有YAML头信息的markdown文件

layout: post
title: 这里是题目
tags:
- 标签1
- 标签2
categories: 分类
description: 描述。

push到github,就能渲染成html
