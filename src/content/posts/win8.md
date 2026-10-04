---
title: Windows 8 Build 779安装教程
published: 2026-09-26
description: Windows 8 7779 在 VMware 中安装流程
tags: [测试版, Windows]
category: 虚拟机
draft: false
pinned: false
---
今天教大家安装**Windows 8 Build 7779**

<div style="position: relative; width: 100%; max-width: 1200px; margin: 1.5rem auto; padding-bottom: 56.25%; height: 0;">
  <iframe
    src="https://player.bilibili.com/player.html?isOutside=true&aid=117336459710829&bvid=BV1AfhR6gEaP&cid=42216393537&p=1"
    scrolling="no"
    border="0"
    frameborder="no"
    framespacing="0"
    allowfullscreen="true"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;">
  </iframe>
</div>

## Part 1.镜像下载
Windows:https://1824041802.share.123pan.cn/123pan/hRnGjv-zV3mA

VMWareTools:https://packages.vmware.com/tools/esx/5.1p09/windows/x64/VMware-tools-windows-9.0.17-3817773.iso

Redlock：https://1824041802.share.123pan.cn/123pan/hRnGjv-bbomA

## Part 2.安装系统
先创建虚拟机，硬件兼容性选择**Workstaion 9.x**

稍后安装操作系统

选择Win7 x64

BIOS引导

CPU核心1核心即可

内存2048MiB

不使用网络连接

接下来默认即可

虚拟机属性里装载Win8 7779 ISO

## Part 3.安装系统

启动时疯狂按F2，进入BIOS

跟着下面的指示，把日期改成2010年7月14日

F10保存

然后跟着指示安装即可

然后安装完先关机

在虚拟机目录的vmx文件下加入以下参数：
time.synchronize.continue = "FALSE"
time.synchronize.restore = "FALSE"
time.synchronize.resume.disk = "FALSE"
time.synchronize.shrink = "FALSE"
time.synchronize.tools.startup = "FALSE"

如果vmx文件里面tools.syncTime是TRUE，改成FALSE

然后再开机

挂载VMWare Tools镜像，安装

装完调整分辨率

哦对了，这个版本开不了Aero