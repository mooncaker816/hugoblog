+++
title = "APUE_With_GO_1"
date = 2018-12-01T10:07:45+08:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["APUE"]
categories = ["C","GO","APUE"]

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
# Use `caption` to display an image caption.
#   Markdown linking is allowed, e.g. `caption = "[Image credit](http://example.org)"`.
# Set `preview` to `false` to disable the thumbnail in listings.
[header]
image = ""
caption = ""
preview = true

+++

# UNIX System Overview：

{{% toc %}}

## 简介

操作系统可以简单地理解为一套用来控制计算机硬件资源并为应用程序提供运行环境的软件，通常我们称这套软件为内核(kernel)。

如下图所示，内核处于整个环境的中心，通过外部包裹的系统调用层(system calls)进行交互。



![](https://notes.shichao.io/apue/figure_1.1.png)

库函数是建立在系统调用层之上的，用户既可以选择调用封装好的库函数，也可以选择直接调用 system calls。

shell，如其字面意思“壳”，不难理解为一个为用户提供交互界面从而来运行其他特定应用的“壳应用”。

更宽泛地说，操作系统是一个内核加上其他一系列为用户提供支持的软件的整体。如人们通常所说的 GNU/Linux，就是以 Linux 为内核的系统。而 Linux 就是由 Unix 演化而来的，有兴趣的同学可以自行google Unix 和 Linux 的历史，也是很有趣的一段过程。

各大厂商在一定的基础上，又根据自身的需求，添加各种相应的软件包，形成了发行版的Linux系统。

## 登录

