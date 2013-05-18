---
layout: post
title: "收集的一些Unity工具栏小插件"
date: 2013-05-12 23:52
comments: true
categories: ['ubuntu','unity','indicator']
---
最近越来越喜欢Unity了，于是找了一些工具栏小插件。

![](http://i.imgur.com/19wWPz9.jpg)

<!--more-->

###天气预报插件(indicator weather)

![](http://i.imgur.com/KODGBn9.png)

安装

	sudo apt-get install indicator-weather

另外有[麒麟版的本地化天气插件][weather]。

[weather]:http://www.ubuntukylin.com/download.html

###监测系统状态(indicator sysmonitor)

![](http://i.imgur.com/OspAjas.png)

安装

	sudo add-apt-repository ppa:alexeftimie/ppa
    sudo apt-get update
    sudo apt-get install indicator-sysmonitor

默认只能显示内存，和cpu状态，可以通过安装Andrew写的脚本显示网络状态。

安装dsat运行脚本

	sudo apt-get install dstat

在主文件夹里面创建一个 “.scripts” 文件夹，并把脚本下载到这个文件夹内

	mkdir -p ~/.scripts && cd ~/.scripts
	wget http://webupd8.googlecode.com/files/sysmon_0.2.tar.gz && tar -xvf sysmon_0.2.tar.gz

然后在indicator-sysmonitor的偏好设置里面新建sensors，在command里输入

	$HOME/.scripts/sysmon

添加到自定义输出，设置开机启动，保存退出。也可以自行配置脚本

	gedit ~/.scripts/sysmon

在脚本开头的位置有下面的几个布尔值，也可以自行添加其他值

	#settings:
	netspeed=true
	ram=true
	cpu=true

###触摸板开关(touchpad indicator)

![](http://i.imgur.com/RQrCL7c.png)

安装

	sudo add-apt-repository ppa:atareao/atareao
    sudo apt-get update
    sudo apt-get install touchpad-indicator

###大小写提示(keylock application indicator)

截不到图，于是网上找一张。<br />
![](http://linux.chinaitlab.com/UploadFiles_7565/201105/2011051711083807.jpg)

安装

	sudo add-apt-repository ppa:tsbarnes/indicator-keylock
    sudo apt-get update
    sudo apt-get install indicator-keylock

(´･ω･`)<br />
以上。
