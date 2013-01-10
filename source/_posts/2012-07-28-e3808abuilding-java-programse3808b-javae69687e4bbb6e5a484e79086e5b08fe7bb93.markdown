---
comments: true
date: 2012-07-28 18:05:24
layout: post
slug: '%e3%80%8abuilding-java-programs%e3%80%8b-java%e6%96%87%e4%bb%b6%e5%a4%84%e7%90%86%e5%b0%8f%e7%bb%93'
title: 《Building Java Programs》-Java文件处理小结
wordpress_id: 238
categories:
- Tips
tags:
- I/O
- 文件处理
---

**写在前面**：文件处理本身并不复杂，但是Java语言并不是为了处理文件而设计的，因此Sun/升阳公司也没有足够的热情来提供一个更简单的解决方法。当然，Sun还是提供了Scanner类，它简化了许多与读取文件有关的操作。总结来讲，**Java的文件处理**（Java I/O）虽然不好用，但是还能用。



	
  1. Java中用File对象代表一个文件，File 类包含在**java.io包**中。

	
  2. Scanner对象可以从文件中读取内容，前提是创建Scanner对象构造函数用"new File(file's name)"作为参数。

	
  3. **可控式异常**（_checked exception_）指在程序执行过程中遇到的一种错误，对这种异常，程序必须有捕捉处理它的代码或显示生命忽略它才能通过编译。例如，创建读取文件内容的Scanner对象时，你必须在main方法头部添加**throws FileNotFoundException语句**。

	
  4. Scanner对象将输入文件视作**一维流数据**，按照从前到后的顺序读取。每次从文件中读出一个标记，输入指针就向前移动。

	
  5. 用于**标记文件内容**的Scanner对象使用一系列**hasNext方法**来检测是否还有更多内容可读。

	
  6. Scanner可以作为参数传递给其他方法（使用[引用传递](http://baham.co/07_25_221.html)），在这些方法内部就可以利用Scanner对象读取文件内容。

	
  7. 文件名可以采用绝对路径，也可以采用相对路径。

	
  8. 很多文件是以行为单位，所以程序也应该可以**逐行**处理文件内容。处理这种情况，经常会用到潜逃循环：外层负责读取文件的每一行，内层负责处理每行内容中的不同标记。

	
  9. 使用**PrintStream对象**可以将结果输出到文件中，创建这样的PrintStream对象时需要提供一个File对象，可以向使用System.out一样使用PrintStream对象，如调用print或者println方法。

	
  10. Java提供了一种**try/catch语句**来检查并处理程序运行过程中发生的错误，try/catch语句可以用来处理找不到要打开指定文件的问题。


_此文系从书中摘录_
