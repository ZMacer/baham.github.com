---
layout: post
title: "Octopress如何做SEO优化"
date: 2013-01-10 17:46
comments: true
categories: [SEO, 站长]
---

对于Wordpress，SEO插件、教程，数不胜数。但是Octopress却几乎没有。
以个人使用到现在的经验，给刚接触Octopress的新手们写些东西。

##1 Robots.txt写法

Octopress的目录结构不同于Wordpress，也不同于国内的CMS，其中javascripts目录,完全没有必要让googlebot索引。
以下为我的robots.txt
{% include_code robots.txt lang:html  %}


仔细想了想，robots.txt也可以这样写-[robots.txt写法](http://baham.co/01_11_octopress-robots-dot-txtxie-fa.html)

##2 Sitemap

还好Octopress默认自动生成Sitemap，所以这点不用担心。

##3 控制垃圾留言

Octopress没有独立的留言系统，不过可以使用Disqus，垃圾信息就交给Disqus自己处理吧。

##4 优化内链

在_include/custom下的footer.html 可以改变foot处的链接。
使用<a href="01_12_octopressxiang-guan-wen-zhang-cha-jian.html">related_posts</a>插件:
以及tag_cloud等插件。


