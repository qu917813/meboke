---
title: Windows CHICAGO Build 58s安装教程
published: 2026-09-12
description: 安装测试版win95 build 58s
tags: [测试版, Windows]
category: 虚拟机
draft: false
pinned: false
---
CHICAGO作为我的**开山之作**，肯定要教一下如何安装

## Part 1: 下载地址
**CHICAGO 58s**：https://winworldpc.com/download/42c2b8c3-90c2-b218-c39a-11c3a4e284a2

**DOS启动盘**：https://1824041802.share.123pan.cn/123pan/hRnGjv-ENKoA

**VMWare想必大家都有**

## Part 2: 虚拟机创建🛠

选择**自定义（高级）**

选择兼容性为Workstation 5.x


选择稍后安装操作系统

版本选择Windows 95

名字瞎取，但不要中文

老系统不支持多核处理器，继续即可

内存其实8MiB就够了（你硬要调64MiB也行，但不要太高，容易进不去）
[![pn3Yum4.png](https://s41.ax1x.com/2026/09/26/pn3Yum4.png)](https://imgchr.com/i/pn3Yum4)

CHICAGO不需要网络（用网络也行，但是我不会）

磁盘相关直接继续就行

## Part 3: 安装虚拟机
添加软盘驱动器
[![pn3Ya0H.png](https://s41.ax1x.com/2026/09/26/pn3Ya0H.png)](https://imgchr.com/i/pn3Ya0H)
[![pn3Y0AA.png](https://s41.ax1x.com/2026/09/26/pn3Y0AA.png)](https://imgchr.com/i/pn3Y0AA)

将**CHICAGO的镜像**装载至**CD/DVD**，**DOS6.22**装载至**软盘驱动器**

启动虚拟机！

然后会来到这里
[![pn3Yy1f.png](https://s41.ax1x.com/2026/09/26/pn3Yy1f.png)](https://imgchr.com/i/pn3Yy1f)

选择第三项

等到出现A:\>_时，输入fdisk分区

然后一路下一步，重启

 再次进入选择第三项。输入format c:格式化C盘。

按回车。

出现警告Y继续

之后转到D盘，输入dossetup开始安装。

按YES

按Customize

下一步

回车继续

等这个死鼓敲好

skip跳过

出现警告，按Cancel取消。
 
按continue 继续。

按ok重启

此时来到这个页面
[![pn3Yy1f.png](https://s41.ax1x.com/2026/09/26/pn3Yy1f.png)](https://imgchr.com/i/pn3Yy1f)

我们关虚拟机，编辑虚拟机配置，把软盘删了
[![pn3YhAs.png](https://s41.ax1x.com/2026/09/26/pn3YhAs.png)](https://imgchr.com/i/pn3YhAs)

再次启动

等待启动完成后按close

遇到这个界面
[![pn3Yo90.png](https://s41.ax1x.com/2026/09/26/pn3Yo90.png)](https://imgchr.com/i/pn3Yo90)

我们第一空填990036

第二空瞎填

哦对了，这个版本装不了VMWare Tools

总体相当于win3.1，但有个屁用也没有的任务栏

WindowsCHICAGO没有自动关机，只是弹出了按Ctrl+Alt+Delete快捷键重启的窗口。（Ctrl+Alt+Delete会对实体机做出反应，对虚拟机需要按软件上的按钮或按Ctrl+Alt+Insert ）

CHICAGO装好了