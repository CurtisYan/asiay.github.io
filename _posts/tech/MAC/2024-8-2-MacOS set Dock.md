---
layout: post
title: 去掉 macOS 中 Dock 栏显示与隐藏时的延迟
category: 技术
tags: tips
keywords: Mac,Dock,setting
description: 
---

>   可能很多朋友使用Mac的时候都会选择将Dock隐藏（可以在系统偏好设置-Dock中选择），等到使用的时候将光标向下一划Dock就会自动弹出显示了。这个显示或者隐藏会有一点点（似乎1秒左右）的延迟，使用下面的方法可以消除这个延迟：
&nbsp;



打开  <mark style="background-color：#D3D3D3">应用程序</mark> - <mark style="background-color：#D3D3D3">实用工具</mark> - <mark style="background-color：#D3D3D3">终端</mark>  

输入如下代码并回车：

  ` defaults write com.apple.Dock autohide-delay -float 0 && killall Dock `

复制代码这样当Dock再次隐藏或者显示的时候就会立即执行的，

如果想要恢复原来默认的延迟速度，就在终端输入如下代码并回车即可：

 `defaults delete com.apple.Dock autohide-delay && killall Dock` 
