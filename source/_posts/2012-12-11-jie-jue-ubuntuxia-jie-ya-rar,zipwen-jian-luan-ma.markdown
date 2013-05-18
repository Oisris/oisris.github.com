---
layout: post
title: "解决Ubuntu下解压rar，zip文件乱码"
date: 2012-12-11 22:28
comments: true
categories: [Ubuntu, 乱码]
---
Ubuntu下解压rar文件出现乱码是因为Ubuntu的unrar是不支持中文编码的，安装Linux版7zip能解决问题。

	sudo apt-get install p7zip p7zip-full p7zip-rar

卸载安装过的rar相关包(如果有安装的话，默认是没有安装的)

	sudo apt-get remove rar unrar

之后，解压rar文件时，归档管理器就会自动调用7z来解压。

<!--more-->

zip文件解压乱码可以参考以上方法卸载unzip让归档管理器选择7z来处理zip文件，也可以使用unzip的`-O CHARSET`选项来指定文件的编码

	unzip -O GBK filename

\_(:3」∠)\_以上。