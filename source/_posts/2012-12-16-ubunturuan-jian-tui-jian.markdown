---
layout: post
title: "Ubuntu软件推荐"
date: 2012-12-16 21:30
comments: true
categories: [Ubuntu,软件]
---
相比Mac和Windows两个平台，Linux下的软件境况真是比较难看了，但也不乏一些比较好用的软件。

### Audacious

Audacious是一款音乐播放软件，对中文支持比较不错，支持GKB等中文编码，支持ape，flac，界面简洁。

![](http://i.imgur.com/DYlTd.png)

<!--more-->

安装

	sudo add-apt-repository ppa:nilarimogard/webupd8
	sudo apt-get update
	sudo apt-get install audacious


### ScreenCloud

ScreenCloud是一个跨平台的截图工具，支持Mac、Windows和Linux，同时提供在线图片分享服务，除了本身的分享服务外还支持FTP和SFTP，另外还支持Dropbox、Imgur、Ubuntu One等第三方存储服务。

![](http://i.imgur.com/nHhYS.png)

官方网站[戳这里](http://screencloud.net)

安装

	sudo apt-get install screencloud

### UberWriter

UberWriter是类似于ReText的MarkDown编辑器，个人感觉界面比较漂亮，但是实用性上还是比不上ReText（<ゝω・）~☆

![](http://i.imgur.com/BO1V7.png)

安装

	sudo add-apt-repository ppa:w-vollprecht/ppa
	sudo apt-get update
	sudo apt-get install uberwriter

这货原来在Ubuntu的商店软件中心还卖5刀呢￢￢

### fcitx+Google拼音+云拼音+Mozc日文输入法

fcitx就是传说中的小企鹅输入法框架，Ubuntu默认的iBus实在是不好用而且难看，fcitx+Google拼音要好很多，而这个Google拼音不是Windows下面的那个Google拼音，这个移植自Android的Google拼音，个人觉得已经很不错了(´°ω°`)

![](http://i.imgur.com/hbB3w.png)

![](http://i.imgur.com/u1OMk.png)

安装

	sudo add-apt-repository ppa:fcitx-team/nightly
	sudo apt-get update
	sudo apt-get install fcitx
	sudo apt-get install fcitx-googlepinyin
	sudo apt-get install fcitx-module-cloudpinyin
	sudo apt-get install fcitx-mozc

只有Ubuntu12.10的源里面才有Mozc的包，12.10以上的版本要修改软件源或者通过编译安装。

可以修改`~/.config/fcitx/config`文件来进行一些设置。

了解详细的编译安装方法可以[戳这里](https://blog.korepwx.com/2012/06/install-fcitx-under-ubuntu-1110/)

以上...
