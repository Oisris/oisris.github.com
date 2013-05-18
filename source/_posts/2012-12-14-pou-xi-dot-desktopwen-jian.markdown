---
layout: post
title: "剖析.desktop文件"
date: 2012-12-14 19:33
comments: true
categories: desktop配置
---

.desktop文件由[Freedesktop.org](http://www.Freedesktop.org)维护，在Gnome，KDE，LXDE，XFCE这些X环境中通用。

.desktop文件有两个主要功能，一个是让程序显示在菜单里面，这需要把.desktop文件放在`/usr/share/applications/`里面，有些特殊情况会放在`$HOME/.local/applications/`里面，另一个功能是让程序显示在桌面，需要把.desktop文件放在`$HOME/Desktop`里面。

.desktop文件的内容按照一个key对应一个value的格式书写：`key=value`

<!--more-->

### 必要元素

Type - 定义条目的类型，有`Application`，`Link`和`Directory`三种。<br />
Name - 定义在菜单或者桌面中显示的名字<br />
Exec - 提供执行命令和相关参数<br />

### 可选元素

Version - 版本信息<br />
Encoding - .desktop文件的编码<br />
GenericName - 定义通用名字（有什么用我也不知道\_(:3」∠)\_）<br />
Nodisplay - 布尔参数，值为`true`的时候图标不在菜单显示，系统认为程序存在<br />
Comment - 可以在这里增加一些说明<br />
Icon - 指图标<br />
Hidden - 布尔参数，值为`true`的时候图标不在菜单显示，系统认为程序不存在<br />
OnlyShowIn - 如果使用多桌面环境（例如同时使用Gnome和LXDE），就可以指定在那个桌面环境显示<br />
NotShowIn - 跟OnlyShowIn相反<br />
Path - 指定默认的工作目录<br />
Terminal - 布尔参数，指定是否需要在终端上运行<br />
Categories - 指定程序属于的类别，详细查看[类别标准](http://standards.freedesktop.org/menu-spec/latest/apa.html)。

可以使用"#"号进行注释

### 例子

创建一个文件`filename.desktop`

``` objc filename.desktop
[Desktop Entry]
Encoding=UTF-8
Version=1.0
Type=Application
Terminal=false
Exec=$HOME/MyApp
Name=Application Name
Icon=$HOME/Icons/MyIcon.png
```

以上...