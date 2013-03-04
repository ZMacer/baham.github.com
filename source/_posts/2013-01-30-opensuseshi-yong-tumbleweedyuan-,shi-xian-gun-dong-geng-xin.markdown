---
layout: post
title: "openSuse使用Tumbleweed源，实现滚动更新"
date: 2013-01-30 16:32
comments: true
categories: [Linux,openSuse]
---

openSuse很早就支持，通过Tumbleweed源，实现滚动更新。
官方Wiki很早就给出了，如何配置，以及注意事项。不过，这段时间使用openSuse的经历，告诉我，Wiki不是总是对的。
至少，我已经发现两处，一是，openSuse Wiki中关于使用Tumbleweed源的问题，一个是在Tumbleweed如何安装Virtualbox。配置Virtualbox，以后再说，今天，先讲讲Tumbleweed源的配置。

![tumbleweed英文Wiki](/images/tumbleweed_en.png )

![tumbleweed中文维基](/images/tumbleweed_zh.png )


<strong>在官方Wiki英文版中，写着要添加4个源。
而中文的，却写着5个。</strong>

后来，我才知道，适用Tumbleweed的关键不是源的多少，像中文wiki中写的,non-oss-current-os源，是后来添加的。但是openSuse英文Wiki并没有添加进去。就像没有维基教程将packman和为Virtualbox准备的虚拟化相关的源添加进去一样。

这些源都是，在Google后openSuse论坛中找到的。

所以，像我之前所说的，不要一切靠Wiki。

现在，Tumbleweed有以下7个源。
(http://download.opensuse.org/repositories/openSUSE:/Tumbleweed/standard/)Tumpleweed最主要的一个源，国内镜像站，均未提供镜像，不过，官方的速度也不慢。

(http://mirrors.sohu.com/opensuse/distribution/openSUSE-current/repo/oss/)

(http://mirrors.sohu.com/opensuse/distribution/openSUSE-current/repo/non-oss/)

(http://mirrors.sohu.com/opensuse/update/openSUSE-current/) 搜狐提供的3个CurrentOs源，速度较快

(http://mirrors.ustc.edu.cn/opensuse/update/openSUSE-non-oss-current/) 中科大的non-oss更新源

(http://packman.inode.at/suse/openSUSE_Tumbleweed) packman的Tumbleweed源

(http://download.opensuse.org/repositories/Virtualization:/VirtualBox_Tumbleweed/openSUSE_Tumbleweed/)虚拟化的源


zypper更新到Tumbleweed时，需要这七个源，其中，后两个是非必须的。


其实，第一次，升Tumbleweed并非因为源的问题，而是因为Wiki中，少写了一步，就是，升级你的软件为当前opensuse版本的最新版，不用补丁最新，只需要软件均为最新。

然后，才可以安全的

`sudo zypper dup --from Tumbleweed `更新到tumbleweed


总结Tumbleweed更新步骤：

##1 更新所有软件为当前版本最新
##2 移出所有当前版本的openSuse源
##3 添加以上七个Tumbleweed需要的源
##4 zypper duo --from Tumbleweed


对于，配置Virtualbox以后再讲。

