---
layout: post
title: "表情绑定工具 Face Combo"
categories: Rigging
tags: [Rigging, Script]
icon: rigging.png
---

---
大家好，今天给大家分享一个表情绑定工具 [Face Combo](https://vimeo.com/251473725)。

![alt text]({{site.url}}/static/assets/img/blog/faceCombo/faceComboTool.jpg "表情绑定工具 Face Combo")

这个工具用来处理两个 BlendShapes 叠加时的效果。比如嘴角向上和嘴角向外组合成的抿嘴笑。我们可以把单个 BlendShapes 调整得很完美，但是当两个 BlendShapes 叠加在一起时，是很难保证组合表情的正确性。我们必须去修复这个表情。不管是用什么方法，根本原理就是表情 A（嘴角向上）和表情 B（嘴角向外）联合驱动表情 C（修型目标体）。

因此，我开发了这个工具，专门用来快速处理这个繁琐的制作工序，使我把注意力集中在表情艺术创作上。我采用了 Maya 自带的 Condition 节点处理联合驱动的数据信息，这比表达式中的 Clamp 函数要快得多，也比独立制作的 Plugin Node 要轻盈，简洁，易于移植。

![alt text]({{site.url}}/static/assets/img/blog/faceCombo/faceComboNodeHierarchy.jpg "Face Combo 节点关系图")

这个工具可以快速创建修型目标体，无限再编辑已经生成的修型目标体，支持删除修型目标体，也支持左右镜像，让表情制作事半功倍。

**Face Combo 主要功能：**
* 基于 Maya 内置的 Condition 节点，干净，整洁；
* 快速创建修型目标体，并自动链接数据信息；
* 无限编辑修型目标体，直到表情修复完美；
* 完美支持删除目标体，自动优化 BlendShapes 节点的 Target 列表；
* 智能镜像修型目标体，无须设置，无论左右，都可以镜像；
* 界面简洁，操作简单，专注艺术创作，表情制作事半功倍。

