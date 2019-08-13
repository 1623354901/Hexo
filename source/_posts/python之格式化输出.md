---
title: python之格式化输出
date: 2018-11-11 19:46:48
tags: 格式化输出
categories: python
cover_picture: https://www.devil.pub/images/feng/python之格式化输出.png
---
如果我们想格式化输出这样一个格式：
{% asset_img 1.png %}
那我们应该怎么操作呢？
下面有三种方法：
第一种：字符串拼接，如图：
{% asset_img 2.png %}
我们看看效果：
{% asset_img 3.png %}
不过这种格式化输出方式需要开辟好多块内存，效率低下，一般不建议使用
第二种：
{% asset_img 4.png %}
我们可以看到，在这种方法里，我们这里用了%做占位符，然后s代表字符，除了s（字符）外，还有d(数字）,f（浮点数）,
但是当我们用到d或者f时一定要给变量强制转换一下变量类型，因为此处变量类型默认str
第三种:format格式
{% asset_img 5.png %}
结果如下：
{% asset_img 6.png %}
在里面，还可以这样：
{% asset_img 7.png %}
以上便是三种格式化方式，个人总结，欢迎各位私聊，深度交流