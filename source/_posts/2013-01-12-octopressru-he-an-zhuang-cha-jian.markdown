---
layout: post
title: "Octopress如何安装插件"
date: 2013-01-12 12:02
comments: true
categories: [Octopress, 开源, 站长]
---

Octopress有如下**目录结构**：
![Octopress目录结构](/images/octopress目录结构.png)

其中plugins就是插件存放地址，
目录里是rb结尾的Ruby脚本，额就是Octopress的插件。


由于插件不同，安装方法也不同，不过大同小异，以下具体说明：

###1 插件只由html文件构成：
如[related-posts](01_12_octopressxiang-guan-wen-zhang-cha-jian.html),只需要将文件复制到对应asides目录，然后配置一下_config.yml即可。

###2 插件由Ruby脚本构成：
多数Octopress插件都是如此，方法相似，只是多了一步，要把对应脚本复制到plugins目录下。


