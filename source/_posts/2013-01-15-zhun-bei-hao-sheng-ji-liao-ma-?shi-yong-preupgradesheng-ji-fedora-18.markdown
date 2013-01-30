---
layout: post
title: "准备好升级了吗？使用Preupgrade升级Fedora 18"
date: 2013-01-15 17:51
comments: true
categories: [Linux, 开源]
---

还有几个小时，Fedora 18的正式版就将释出。

Fedora 18的桌面环境默认是[Gnome3.6](https://fedoraproject.org/wiki/Features/Gnome3.6)，而且全新加入了Gnome 2的分支[Mate](https://fedoraproject.org/wiki/Features/MATE-Desktop)，终端可以使用256色替代旧的8色。firewalld成为默认的防火墙。而且更新了Samba到4……


使用preupgrade只适用于Fedora 17 及以前版本，不再适用于Fedora 18.
## 1 备份
（在任何系统的变动前，推荐进行备份，虽然多数情况下，不备份，并不会毁掉你的数据，此处，还是老声长谈，备份你的重要数据）
## 2 更新一切可更新内容
`yum update`
## 3 安装preupgrade
自从fedora10之后，preupgrade都会被默认安装。此处也可手动安装
`yum install preupgrade`
## 4 开始更新
在终端中运行  `preupgrade`
## 5 配置preupgrade及更新安装fedora 18
![preupgrade 1](/images/preupgrade1.png)

点击 forward
<!-- more -->
![preupgrade choose system](/images/preupgrade2.png)

选择系统，此处以Fedora 17为例。
点击 Apply

![preupgrading](/images/preupgrade3.png)

升级更新中

![preupgraded and reboot](/images/preupgrade4.png)

重启系统

![grub choose update](/images/preupgrade5.png)

Grub菜单中 选择 对应 update选项,此处以Fedora  17为例。


至此。Fedora更新完成。Fedora 18不支持使用preupgrade更新与此相同。
当然，也可以使用更稳妥的刻盘升级，以及较复杂的yum更新方法。
相应资料，可寻找fedora对应Wiki文档
