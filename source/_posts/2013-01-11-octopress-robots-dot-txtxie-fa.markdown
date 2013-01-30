---
layout: post
title: "Octopress robots.txt写法"
date: 2013-01-11 22:23
comments: true
categories: [SEO, Octopress, 站长]

---


又想了想Octopress的robots.txt写法。
现在我的是这样：
{% codeblock  %}
User-agent: *
Disallow: /*?*
Disallow: /archives
Disallow: /javascripts
Disallow: /font
Disallow: /assets
Disallow: /blog
Sitemap: http://baham.co/sitemap.xml
{% endcodeblock %}
Line 1:对于所有搜索引擎

Line 2:禁止访问所有动态内容（虽然Octopress的文章都是纯净态，但是此处还是加上，比如我在用Cloudflare时，Cloudflare默认就会生成一些带?的缓存链接）

Line 3～7:禁止访问archives,javascripts,font,assets,blog目录，archives是归档内容，blog目录下是归档内容以及分类内容和页号内容，由于更新较频繁，建议禁止。

Line 8: sitemap地址

