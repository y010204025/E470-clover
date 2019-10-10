下次更新，看心情啦。

# 更新说明：
1.更新clover到最新的clover r5093,目前测试版本为10.15beta11,各种驱动更新到10月7日最新版。

2.使用AptioMemoryFix.efi，这个感觉兼容性不错的。

3.将fakesmc切换到virtualsmc,并加入了电池、传感器相关驱动，目前测试运行正常，传感器驱动正常。

4.在config.plist/boot/Arguments加入了启动参数：-lilubetaall brcmfx-country=#a

5.蓝牙不可用，更换为可用版本，需要到Windows下面用一次蓝牙才能正常使用。嫌麻烦的自己去找解决方案。

参数说明：本次新增的-lilubetaall是10.15所必须的，brcmfx-country=#a这是解决无线网络5G信号的地区差异的，支持5G所有频段。

OneNote教程类：https://1drv.ms/u/s!AnZiqbrvoEVXicJ9ainApP52bzmH5A

# 关于 10.15 的小贴士
1.针对10.15beta系统分区不可写入的问题，可以在终端执行以下命令：sudo mount -o rw /

2.允许未知软件运行(全新安装必须运行)：sudo spctl --master-disable

3.解除4位密码限制：pwpolicy -clearaccountpolicies

4.如果在启动台不显示应用程序：可以把对应的应用程序拉到启动台图标上，然后执行以下命令：
rm ~/Library/Application\ Support/Dock/*.db
killall Dock

5.10.15安装过程中存在的问题和解决办法请参照黑果小兵博客：
https://blog.daliansky.net/Common-problems-and-solutions-in-macOS-Catalina-10.15-installation.html

6.添加noTouchID.kext，解决输入密码前的卡顿。

# 各种致谢大佬：

感谢rehabman(https://github.com/RehabMan?tab=repositories) 、宪武、vit9696(虽然对此大佬不感冒)(https://github.com/vit9696?tab=repositories)

黑锅小兵(背的锅不少)(https://github.com/daliansky?tab=repositories) 、tluck(ThinkPad 主题提供者)(https://github.com/tluck?tab=repositories)
还有其他的啦。


