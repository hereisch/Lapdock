# 不连接手机使Motorola Lapdock500 作为外接显示器

## Makes the Motorola LapDock500 serve as an external display without connect phone

​	PS:本文需一定动手能力。希望给手里有Lapdock500的盆友一些帮助。

​	之前淘了一部Motorola的Lapdock500，本想着作为外接显示器和usb hub使用(还自带电池)，但这玩意需要连接手机(XT910/MT917)才能使用，无奈又搞了一部二手手机，每次使用时必须连接手机才能使lapdock正常工作，很是繁琐，且USB hub、键盘、触摸板功能都无法使用![lapdock](https://ww4.sinaimg.cn/mw690/c605728egw1famouykgcoj21kw16owxi.jpg)。

​	最近在油管上看见国外大神[使用Lapdock500 作为树莓派的外接显示器](https://www.youtube.com/watch?v=-a3qS45Z_ro)，且不用连接手机，于是淘了一些元件开干！！！

## 原理图

​	![原理图](https://wx2.sinaimg.cn/mw690/c605728ely1gmz2cpr546j20rl0lbwjj.jpg)

​	简单地说，就是短接Micro USB母端的Vcc和ID引脚。查了一下Micro USB的引脚定义和OTG线连接方法，ID要么脚接地(client/peripheral mode)，要么浮空(host mode)。这ID上电是什么操作？

## DIY



![所需元件](https://wx1.sinaimg.cn/mw690/c605728ely1gmz1p68gnbj20u0140x6p.jpg)

​	所需元件：Micro USB五芯母线(必须是五芯)、开关按键、USB测试板、热缩管若干、耐心

​	根据大神提供的原理图:

​	1.将Micro USB母线的GND、D+、D-端与USB测试板对应的引脚焊接起来。

​	2.将Micro USB母线的Vcc和ID脚分别焊接至按键开关的同侧引脚上。

​	注意：要焊接至按键开关的同侧引脚(13或24)

​	![按键开关引脚](https://wx3.sinaimg.cn/mw690/c605728ely1gmz3bywzelj204y02jdfn.jpg)

​	![1](https://wx4.sinaimg.cn/mw690/c605728ely1gmz1qigl8gj20u0140b2a.jpg)

​	![2](https://wx2.sinaimg.cn/mw690/c605728ely1gmz2bozssaj20u01404qq.jpg)

​	![3](https://wx3.sinaimg.cn/mw690/c605728ely1gmz1rf1obsj20u0140x6p.jpg)

​	

## 成果

​	连接主机，按下开关实现外接显示器、键盘、触摸板、USB hub、读卡器等集成外设 :)。

​	![效果1](https://wx4.sinaimg.cn/mw690/c605728ely1gmz2c192xyj21400u0x6p.jpg)

​	![效果2](https://wx2.sinaimg.cn/mw690/c605728ely1gmz2c9x53vj20u01407wi.jpg)




