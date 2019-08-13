---
title: win10打开hyper-v方法及安装centos方法
date: 2018-11-14 22:31:35
tags: hyper-v
categories: 虚拟机
cover_picture: https://www.devil.pub/images/feng/win10打开hyper-v方法及安装centos方法.png
---
一、win10打开hyper-v方法：

先找到控制面板，然后选择程序，打开或关闭windows功能：
{% asset_img 1.png %}
点击确定后重启电脑，就可以找到hyper-v管理器：
{% asset_img 2.png %}
二、虚拟交换机联网：

双击打开，然后选择连接到服务器，选择本地计算机，确认：
{% asset_img 3.png %}
然后为虚拟交换机配置网络：选择虚拟交换机管理器--外部--创建
{% asset_img 4.png %}
然后出来这个界面：
{% asset_img 5.png %}

三、创建虚拟机：

选择新建，虚拟机：出来安装向导：
{% asset_img 6.png %}
点击下一步，然后为它命名，并选择安装位置：
{% asset_img 7.png %}
代数指定第一代：
{% asset_img 8.png %}
根据实际选择内存
{% asset_img 9.png %}
然后网络连接选择虚拟交换机：
{% asset_img 10.png %}
选择虚拟硬盘，并选择硬盘大小
{% asset_img 11.png %}
安装选项选择CD/DVD安装，然后选择映像文件，找到自己下载好的映像文件：
{% asset_img 12.png %}
看看摘要，确定没问题的话点击完成：
{% asset_img 13.png %}
四、安装centos7
先点击连接，然后点击开关
{% asset_img 14.png %}
选择语言，中英文都可：
{% asset_img 15.png %}
设置完用户密码就耐心等待，然后重启就可以啦！！