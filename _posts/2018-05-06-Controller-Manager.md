---
layout: post
title: "控制器工具 Control Manager"
categories: Rigging
tags: [Rigging, Script]
icon: rigging.png
---

---
![alt text]({{site.url}}/static/assets/img/blog/controlManager/controlManager.jpg "表情绑定工具 Face Combo")

大家好，今天给大家分享一个控制器相关的工具 Control Manage。

正如图片中的效果显示，简单的可以分为三个部分：Change Color，Change Shape， Adjust Shape。

Change Color 里的颜色表是和 Maya 的 Drawing Overrides - Color 属性对应的，根据实际需求可以在 Transform 或 Shape 节点上改变控制器颜色。

Change Shape 就是这个工具的重点了。Add 是指在控制器上添加一个新的控制器形态。Create 是指创建一个新的控制器， Replace 是指替换一个控制器的形态。

Adjust Shape 目前有两个功能，通过滑竿调整控制器形态的大小和镜像相同点数的控制器的形态，后面会继续完善这些功能。


**Control Manager 功能：**
* 生成多种形态的控制器；
* 批量修改控制器的颜色；
* 批量替换控制器的形态；
* 批量添加控制器的形态；
* 缩放控制器形态的大小；
* 多轴向镜像控制器形态。

