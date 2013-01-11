---
layout: post
title: "Github绑定域名"
date: 2013-01-10 22:35
comments: true
categories: [Github, 开源]

---

1 创建CNAME在你的repo
此处CNAME指的是一个文件，文件名即CNAME，在其中，填入你想要绑定的域名。
比如本站：
{% blockquote %}
baham.co
{% endblockquote %}

2 配置DNS
配置A记录到  204.232.175.78

CNAME   www.xxx.com 到  name.github.com


github英文帮助内容-<a href="https://help.github.com/articles/setting-up-a-custom-domain-with-pages">custom domain</a>


