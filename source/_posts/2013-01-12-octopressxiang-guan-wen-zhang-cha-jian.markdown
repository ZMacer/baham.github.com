---
layout: post
title: "Octopress相关文章插件"
date: 2013-01-12 11:44
comments: true
categories: [SEO, Octopress]

---

默认，Octopress没有*相关文章插件*。不过，有人为Octopress写了一个[relatedposts](https://github.com/jcftang/octopress-relatedposts.git)

演示可以看本站右下位置。

相应的配置安装也很简单。

##1 配置_config.yml

添加`lsi: true`。


##2 设置侧边栏

在default_asides中添加`custom/asides/related.html`

##3 添加插件

复制[压缩包](https://nodeload.github.com/jcftang/octopress-relatedposts/zip/master)内的related.html文件到这里 source/_includes/custom/asides/related.html 


至此Octopress的相关文章插件，配置完成。
