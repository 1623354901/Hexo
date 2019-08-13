---
title: 使用win7超级终端连接华为交换机并配置端口镜像
date: 2018-11-11 20:06:57
tags: 端口镜像
categories: 网络
cover_picture: https://www.devil.pub/images/feng/使用win7超级终端连接华为交换机并配置端口镜像.png
---
 首先，用console连接主机和交换机，打开超级终端，（注意：一定要用win7系统配置）如图所示：
{% asset_img 1.png %}
{% asset_img 2.png %}
新建连接时名字随意，但要注意不能是下面图标：
{% asset_img 3.png %}
然后出现下面这样一个页面，连接时使用COM1口，也可通过此电脑--右键管理--设备管理器--端口查看端口号，如图：
{% asset_img 4.png %}
{% asset_img 5.png %}
点击确定，出现这样一个界面：
{% asset_img 6.png %}
设置中终端参数为默认值，即：波特率：9600bit/s,数据位8位，一位停止位，无校验和无控制流。如下图：
{% asset_img 7.png %}
点击完成后进入以下界面：
{% asset_img 8.png %}
此时再插上交换机的电源，（提前插上会出现键盘失灵的情况），终端上显示以太网交换机自检信息，自检结束后提示用户输入回车，到现在，超级终端和交换机之间的连接已经建立好了，接下来进行配置：
1.输入用户名，密码，华为新交换机默认用户名：admin,密码:admin@huawei(说明书上也有）.
{% asset_img 9.png %}
2.接下来进入用户模式：system-view：
(注意：思科有用户模式，特权模式，全局配置模式三种，
enable：从用户模式进入特权模式
configure terminal：进入全局配置模式）
华为有用户视图和系统视图两种：
system-view：从用户视图到系统视图
quit：从系统视图退到用户视图）
{% asset_img 10.png %}
3、配置观察口和镜像口，在这里，我设置1口为观察口，监控流量，2.4.6.7.8为镜像口，
配置观察口命令：observe-port interface GigabitEthernet0/0/1
{% asset_img 11.png %}
配置景象口命令：
端口2：interface GigabitEthernet 0/0/2 
Port-mirroring to observe-port 1 both (both指对流入和流出的数据包都进行映射，inbound为对进入的映射，outbound流出映射，这里我们选择bound) 
其他镜像端口同上，如图：
{% asset_img 12.png %}
这样镜像端口就配置成功了。
