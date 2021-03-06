---
layout: post
title: MVC和MVVM关系及对比
date: 2016-08-22 00:00:00
tags: 架构
---

### 关系：

**M-V-C**：model - **view - controller**

**M-V-VM**：model - **view/viewController** - viewModel

### 一、本质：

比较MVC和MVVM之后：其实MVVM是在MVC的基础上增加了VM层

### 二、分析：

1、将原MVC的**V和C**统一归为**V**，即原MVC被简化为：**M-V**

2、再在简化后的础上添加VM层，即：**M-V** - VM

### 三、图例（截图取自objc.io）:

##### 1、标准MVC：

![img](/assets/images/2016/MVC和MVVM-1.png)

##### 2、MVC简化为MV：

![img](/assets/images/2016/MVC和MVVM-2.png)

##### 3、MV添加VM变为MVVM：

![img](/assets/images/2016/MVC和MVVM-3.png)