---
layout: post
title: "从Wordpress转移到Octopress"
date: 2013-01-10 15:50
comments: true
categories: [Baham, Tips, 站长]
---

一直在用wordpress，最近Godady的空间即将到期，迁移到了openshift上，结果很悲剧，莫名其妙的出现502错误，之后又是500错误。既然如此，索性就不用WP了。
但是wordpress上的内容还是想保留的，毕竟辛辛苦苦写半年博客了。
在谷歌搜索到了相关迁移的文章。

需要使用<a href="https://github.com/thomasf/exitwp.git">exitwp</a>，很好用的脚本，python写的。
可以参考<a href="/files/Migrating Wordpress blogs to Octopress.pdf">这篇文章</a>。
当然，一切不会那么顺利。

我上传到新博客后，发现链接全变了。而且，也不是所有内容都转移到了新的地址上。
我的wp用的固定链接为-月日postid。
但是octopress没有postid这一概念。困惑我很久，后来，在exiwp.py代码中找到了玄机，我将title和wp_id属性稍微改动了一下，结果在build文件夹中的内容全变成了以worpdress的postid命名的文章。

不过，随后又有问题出现，由于写博客多数时间在晚上。我发现，很多地址中‘月日’部分比在wordpress的链接地址多一天，显然时区不对。

在谷歌搜索后，找到了解决方案。
使用
{% codeblock %}
TZ=CCT rake generate
{% endcodeblock %}


代替rake generate

ps：   cct：表示中国东部标准时。

随后添加了一些插件什么的，一个崭新Octopress就这么诞生了。相较于wp，可能显得复杂、简单了一些，不过，还不错而且更快。

一些关于Octopress和github的内容，以后再和大家分享，敬请期待！！！

——Baham
