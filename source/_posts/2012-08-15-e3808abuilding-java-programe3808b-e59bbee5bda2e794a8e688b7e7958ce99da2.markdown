---
comments: true
date: 2012-08-15 22:09:05
layout: post
slug: '%e3%80%8abuilding-java-program%e3%80%8b-%e5%9b%be%e5%bd%a2%e7%94%a8%e6%88%b7%e7%95%8c%e9%9d%a2'
title: 《Building Java Program》-图形用户界面小结
wordpress_id: 424
categories:
- Tips
tags:
- GUI
---


	
  1. Java中所有图形组件拥有共同的继承结构，所以它们都包含一些可以对属性进行访问和设置的共同函数，比如背景颜色、大小、字体等。

	
  2. 组件被**布局管理器（Layout Manager）**放在**框架（Frame）**或其他容器之中，比如BorderLayout、FlowLayout、GridLayout。通常把不同的布局管理器借助不同的容器进行嵌套以构成**复合布局**。

	
  3. 当用户与屏幕上显示的图形组件进行交互时，Java会产生一种叫做**事件（Event）**的特殊对象。为了构建一个交互式GUI，必须对这些时间进行响应。

	
  4. 最常见的事件是**ActionEvent**，可以通过编写一个实现MouseListener接口的类来处理它。也可以编写一个对MouseInputAdapter类进行了扩展的雷来实现对MouseEvent的响应。

	
  5. 为了绘制图形和线条，我们需要扩展JPanel类，并构建paintComponent方法。

	
  6. 可以使用timer对象实现动画。


