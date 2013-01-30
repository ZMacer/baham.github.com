---
layout: post
title: "使用fedup从Fedora 17更新到 Fedora 18"
date: 2013-01-15 23:29
comments: true
categories: [Linux, 开源]

---

##1 联网升级

适用于网速较好，且网络环境稳定的用户。

	sudo fedup-cli --network 18 --debuglog fedupdebug.log --instrepo http://dl.fedoraproject.org/pub/alt/qa/fedup/f18-RC4/<arch>/

`arch 请填写处理器架构——  i386  or X86_64`

其中，地址部分，此处为RC版。

以上为原RC版升级方案，正式版范例如下。

更新 fedora 18 使用以下命令：
	sudo fedup-cli --network 18 --debuglog fedupdebug.log


`其中arch表示处理器架构。`

对应wiki：[Fedora fedup  wiki](https://fedoraproject.org/w/index.php?title=FedUp&action=history)

##2 ISO(DVD版)  升级

适用于网络环境稳定性较差或者网速较慢时。

	sudo fedup-cli --iso /home/name/download/fedora-18.iso --debuglog=fedupdebug.log



DVD iso 下载地址  (163源  http://mirrors.163.com/fedora/releases/18/Fedora/x86_64/iso/Fedora-18-x86_64-DVD.iso)。


其中fedupdebug.log用于记录升级过程日志。

fedup帮助文档（英文）:
<!-- more -->

{% blockquote %}
usage: fedup SOURCE [options]

Prepare system for upgrade.

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose         print more info
  -d, --debug           print lots of debugging info
  --debuglog DEBUGLOG   write lots of debugging output to the given file
  --reboot              automatically reboot to start the upgrade when ready

SOURCE:
  Location to search for upgrade data.

  --device [DEV]        device or mountpoint. default: check mounted devices
  --iso ISO             installation image file
  --network VERSION     online repos matching VERSION (a number or "rawhide")

additional options for --network:
  --enablerepo REPOID   enable one or more repos (wildcards allowed)
  --disablerepo REPOID  disable one or more repos (wildcards allowed)
  --addrepo REPOID=[@]URL
                        add the repo at URL (@URL for mirrorlist)
  --instrepo REPOID     get upgrader boot images from REPOID (default: auto)

cleanup commands:
  --resetbootloader     remove any modifications made to bootloader
  --clean               clean up everything written by fedup
{% endblockquote %}

[fedup英文Wiki](https://fedoraproject.org/wiki/FedUp)

