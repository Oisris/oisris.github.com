---
layout: post
title: "Sublime text，又一个编辑利器"
date: 2013-05-13 15:57
comments: true
categories: ['sublime','软件']
---
[Sublime](http://www.sublimetext.com/)是个跨平台文本编辑器，有丰富的插件支持，在Linux和windows下都有很好的表现。界面很好看，尤其右边的缩略图在看打文件时实在美爆了>_<。而且Sublime在使用[zencode](https://code.google.com/p/zen-coding/)的时候能看实时效果。看过[Lucifr](http://lucifr.com/)大大的一些介绍之后更是觉得碉堡。

![](http://i.imgur.com/138orcg.png)

可以在官网[下载](http://www.sublimetext.com/2)，直接解压可用。

也可以添加ppa源安装

	sudo add-apt-repository ppa:webupd8team/sublime-text-2
	sudo apt-get update
	sudo apt-get install sublime-text

安装Package Control，<code>ctrl+`</code>打开控制台，输入

	import urllib2,os;pf='Package Control.sublime-package';ipp=sublime.installed_packages_path();os.makedirs(ipp) if not os.path.exists(ipp) else None;open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read())

然后可以通过Package Control方便地安装插件了。
更多有趣的使用方法可以参考[Lucifr的博文](https://www.google.com/search?q=sublime&q=site%3Alucifr.com).
