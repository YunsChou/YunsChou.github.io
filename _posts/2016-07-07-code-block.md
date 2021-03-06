---
layout: post
title: block和C语言函数对比
date: 2016-07-07 00:00:00
tags: code
---

## 目的

通过对比block和C语言函数，理解block是`函数指针`的概念

[DEMO点我](https://github.com/YunsChou/ExercisProject/tree/master/链式函数式响应式编程/EX-RAC-DEMO/block和C函数)

## 何为block

1. block就是`函数指针`，可以将函数当做`变量、参数`来传递
2. block是一个`OC对象`，它的功能是`预先保存代码片段，并在需要的时候执行`
3. block的出现主要是用来弥补OC中没有（lambda，闭包或者说匿名函数）的语言特性，为`函数式编程`提供了可能（通俗的讲，就是弥补OC中没有：`将一个函数作为参数和变量来使用`，这种语言特性）
4. 在下面的截图中，`int (^minBlock)(int a, int b)`是一个block，但也可以理解为：**将名字叫做minBlock的函数，保存在一个指针中，这个函数可以当做OC的参数和变量来使用**

![img](/assets/images/2016/block和C语言函数对比-1.png)

## block和函数的区别

1. 相同点：block和函数都是`先创建，再调用`，参数都是放在`block名`或`函数名`之后
2. 不同点：函数是在编译的时候就被保存了，block是运行的时候才去定义