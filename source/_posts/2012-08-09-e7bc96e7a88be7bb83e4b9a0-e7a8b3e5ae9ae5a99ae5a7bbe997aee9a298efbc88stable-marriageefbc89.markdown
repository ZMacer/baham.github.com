---
comments: true
date: 2012-08-09 22:06:35
layout: post
slug: '%e7%bc%96%e7%a8%8b%e7%bb%83%e4%b9%a0-%e7%a8%b3%e5%ae%9a%e5%a9%9a%e5%a7%bb%e9%97%ae%e9%a2%98%ef%bc%88stable-marriage%ef%bc%89'
title: 编程练习-稳定婚姻问题（Stable Marriage）
wordpress_id: 402
categories:
- Java练习题
tags:
- Java集合框架
- 稳定婚姻
---

对于给定的一群男女，在他们当中建立尽可能多的**稳定婚姻**。如果现在一对夫妻能找到比他们的配偶更适合的异性，则他们的混为**不稳定婚姻**。

输入文件中所有男人信息放在一起，没人一行，然后是空行，后面是女人的信息，也是没人一行。每个人根据他们的行号进行编号（如，第一个男人为1号）。输入文件的每一行的开头都是人命（男女间空行除外），后面是冒号，在后面是**一串整数**，用以保存每个人对配偶的偏好。例如：

Java: 10 8 5 6

名为**Java**的人，和异性中10号是最好的组合，8号其次，不再列表上的无法组合。

完整示例如下：<!-- more -->

    
    //输入内容如下



    
    Man1: 4 1 2 3
    Man2: 2 3 1 4
    Man3: 2 4 3 1
    Man4: 3 1 4 2
    
    Woman1: 4 1 3 2
    Woman2: 1 3 2 4
    Woman3: 1 2 3 4 
    Woamn4: 4 1 3 2




    
    //输出内容如下：
    
    Man1 and Woman4
    Man3 and Woman2
    Man2 and Woman3
    Man4 and Woman1
