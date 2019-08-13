---
title: 在服务器里安装Linux系统(centos7)
date: 2018-11-14 19:40:23
tags: Linux
categories: Linux
cover_picture: https://www.devil.pub/images/feng/在服务器里安装Linux系统(centos7).png
---
首先，进入VMware Vsphere Client，软件如图所示：
{% asset_img 1.png %}
点击进入，如图：
{% asset_img 2.png %} 
ip地址为你在虚拟控制台设置的地址，用户名默认root,密码也是你设置的密码。

进入之后是这样一个页面：
{% asset_img 3.png %}
要想安装Linux系统，首先上传centos镜像到服务器：
点击配置，存储，右击，浏览数据存储：
{% asset_img 4.png %}
{% asset_img 5.png %}
点击上传文件至服务器，
{% asset_img 6.png %}
上传完之后，点击创建虚拟机：
{% asset_img 7.png %}
{% asset_img 8.png %}
输入名字：
{% asset_img 9.png %}
选择资源池：
{% asset_img 10.png %}
{% asset_img 11.png %}
选择客户机操作系统和版本
{% asset_img 12.png %}
{% asset_img 13.png %}
一定要勾上打开电源时连接。
创建磁盘时要选择厚置备延迟置零：
{% asset_img 14.png %}
{% asset_img 15.png %}
点击完成，创建成功，现在虚拟机就配置成功了.
右击虚拟机，里面有编辑设置，可根据需求对虚拟机进行配置，注意，驱动器那要选择数据存储iso
{% asset_img 16.png %}
接下来就是安装了，点击左侧你命名好的的虚拟机，然后点击控制台，点击左上角绿色三角：
{% asset_img 17.png %}
等待以后，进入这样一个界面：
{% asset_img 18.png %}
最好时选择英文，不过中文也是可以的。
然后就进入安装信息摘要了：
{% asset_img 19.png %}
注意软件选择里选择GNOME桌面，默认的是最小安装，不适用于初学者。右边可根据需要选择。
{% asset_img 20.png %}
都配置好之后点击开始安装：
在这设置root密码，创建用户：
{% asset_img 21.png %}
配置完成后，等待安装，成功后点击重启：
{% asset_img 22.png %}

这样就安装好了。

 
