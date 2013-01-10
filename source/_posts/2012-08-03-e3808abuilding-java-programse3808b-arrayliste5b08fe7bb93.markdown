---
comments: true
date: 2012-08-03 19:52:23
layout: post
slug: '%e3%80%8abuilding-java-programs%e3%80%8b-arraylist%e5%b0%8f%e7%bb%93'
title: 《Building Java Programs》-ArrayList小结
wordpress_id: 353
categories:
- Tips
tags:
- ArrayList
---

_java.util_包中的**ArrayList**类表示一个大小可以自动增长的对象列表，它在内部用数组来实现这个列表。可以用ArrayList顺序地保存对象元素，其元素索引从0开始。



	
  1. ArrayList是一个**泛型类**，创建泛型类对象时需要指定一种数据类型，例如，**ArrayList<String>**。

	
  2. ArrayList可以自己维护列表的大小，可以在任何索引位置插入或删除元素。ArrayList还支持_get、set、clear、、toString_等方法。

	
  3. 可以用_contains、indexOf、lastIndexOf_方法查找ArrayList中的元素。

	
  4. 可以用**for-each循环**来**遍历**ArrayList中的元素。但在这个过程中不能修改列表的内容。

	
  5. 如果要在ArrayList中保存基本类型的数据，如int或double等，就必须在创建对象时，使用其对应的**包装类**，如Integert和Double。

	
  6. **Comparable接口**定义了可以实现自然排序的compareTo方法。实现了Comparable接口的类可以保存到ArrayList对象中，很多常用类型（如：String，Integer）都实现了Comparable接口，也可以在自定义类中实现Comparable接口。


