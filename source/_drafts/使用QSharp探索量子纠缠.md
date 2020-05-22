---
title: 在VSCode中安装Q#
date: 2020-04-05 22:36:52
tags:
    - QSharp
    - Python
    - VSCode
    - 量子
categories:
    - IT
    - QSharp
id: ExploreQuantumEntanglement
copyright: true
---

>在上一篇文章中我简单介绍了如何在个人计算机上安装量子程序开发环境，那么在这篇文章中我将介绍如何使用Q#来开发软件，并探索量子力学中的纠缠态！

<!--more-->

>声明：本文部分内容转载自[微软官方文档](https://docs.microsoft.com/zh-cn/quantum/quickstart?tabs=tabid-python)。

# 准备工作

首先打开VSCode（哦天哪我又说了一句废话......），在你喜欢的地方建个文件夹（名称随意，为了后面操作方面建议使用英文，such as `Entanglement`）

然后在文件夹下建两个文件`Operation.qs`（.qs文件为Q#源码的后缀名，在它里面编写Q#的算法）`host.py`（主机程序，通过它来调用你在qs文件里面写的量子算法，即量子程序）

# 思想工作

好吧，我承认，这个标题写的有点无聊，但是它很重要！要知道，量子力学和经典力学几乎不是一回事！

在经典力学的环境下，计算机的指令由0和1组成，亦成称之为二进制。它只有0或1两种状态。但是在对于量子世界，一个“量子位”的状态