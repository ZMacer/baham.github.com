---
comments: true
date: 2012-07-29 00:42:26
layout: post
slug: iqq-%e5%bc%80%e6%ba%90java%e7%89%88qq%e5%ae%a2%e6%88%b7%e7%ab%af
title: iQQ-开源Java版qq客户端
wordpress_id: 251
categories:
- Java
- Linux
- 源码
tags:
- iQQ
---

![iQQ登陆界面](https://iqq-java.googlecode.com/files/loginProccess.jpg)        用过Linux的都知道，QQForLinux处于长期不更新状态，而且存在很多小bug，并且很多QQ该有的功能都没有。于是乎，许多人开始使用第三方QQ插件，比如[libqq-pidgin](http://libqq-pidgin.googlecode.com/)，不得不说pidgin是一款很好的IM软件，但libqq-pidgin和QQforLinux一样，很多小问题没有解决。问题主要原因显然不在软件，而在腾讯方面。

今天无意中，看到了iQQ的介绍，这是一个新项目，距离谷歌Code的项目提交只有几天。看了一些iQQ的截图，至少觉着这个图形界面，要比QQforLinux或者其他第三方客户端要好那么一点。

iQQ是一项**开源项目**，源码托管在google code上，基于腾讯**WebQQ 3.0网络协议**，可以通过JRE运行在任何平台上，作者基于Linux(Ubuntu 12.04)系统，使用IDE NetBeans开发。项目伊始，作者（_chengnuo128@gmail.com_）将源代码公开，希望寻找爱好者一同开发。

截至目前，iQQ仍处于**Beta测试**阶段，通过项目问题也看到，仍有部分小问题没有解决。

<!-- more -->

iQQ截图：

![xfce ubuntu12.04 iqq客户端](https://iqq-java.googlecode.com/files/mainFrame.jpg)

![](https://iqq-java.googlecode.com/files/cap.jpg)

![iQQ登陆界面](https://iqq-java.googlecode.com/files/login.jpg)

![iqq使用界面](https://iqq-java.googlecode.com/files/1.jpg)

![iqq聊天示例](https://iqq-java.googlecode.com/files/chating.jpg)

总结来讲，我很看好**iQQ项目**，虽然我还不能为其贡献代码，但真心希望有兴趣者积极参加。没有什么别的原因，只是希望Linux的桌面应用能更丰富。

[iqq项目地址](https://code.google.com/p/iqq/)

[iqqBeta1.02下载地址](https://code.google.com/p/iqq/downloads/detail?name=iQQ_beta1.02.zip&can=2&q=)

获取iqq源代码：

`# Non-members may check out a read-only working copy anonymously over HTTP.
svn checkout http://iqq.googlecode.com/svn/trunk/ iqq-read-only`
