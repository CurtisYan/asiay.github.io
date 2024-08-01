---
layout: post
title: Mac系统安装APP时打开报错：文件已损坏
category: 技术
tags: tips
keywords: Mac,file,setting
description: 
---

<big>**Mac系统安装APP时打开报错：文件已损坏，您应该将它移到废纸篓**</big>

<big>**解决办法**</big>

  

* 打开终端输入以下内容，“为安装路径，默认是以下路径”



` sudo xattr -d com.apple.quarantine "/Applications/<u>*APP*</u>.app" 

  

* 按照提示输入电脑锁屏密码回车即可
