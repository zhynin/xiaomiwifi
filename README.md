# xiaomiwifi

dogcom，仅一个大小为几十 KB 的二进制文件(可执行文件) 适用于几乎所有路由器 已测试支持斐讯 K2、小米 mini、小米路由器 3、小米路由器 3G、New-wifi、极路由等路由器

一、连接路由器

登录192.168.1.1
or
[http://miwifi.com/cgi-bin/luci/web/init/hello](http://miwifi.com/cgi-bin/luci/web/init/hello)

同意 -> 设置账号密码（asd11096） -> 设置管理密码 （默认选择与WiFi密码相同） 

二、刷官方网站

下载

下载 ROM for R3 开发版

回到管理页面，点击系统升级，手动，刚才下载的文件。

大约3分钟

三、下载工具

下载xiaomiwifi 然后登录绑定

[https://d.miwifi.com/rom/ssh](https://d.miwifi.com/rom/ssh)

找到，然后下载


然后。。。。

工具包使用方法：小米路由器需升级到开发版0.5.28及以上，小米路由器mini需升级到开发版0.3.84及以上，小米路由器3即将支持。注意：稳定版不支持。
请将下载的工具包bin文件复制到U盘（FAT/FAT32格式）的根目录下，保证文件名为miwifi_ssh.bin；
断开小米路由器的电源，将U盘插入USB接口；
按住reset按钮之后重新接入电源，指示灯变为黄色闪烁状态即可松开reset键；
等待3-5秒后安装完成之后，小米路由器会自动重启，之后您就可以尽情折腾啦 ：）


然后ssh root@192.168.31.1连接

连不上就删除对应的ip
~/.ssh/known_hosts


把dogcom和drcom.conf放入/data/
chmod 755 dogcom

firewall.user放入/data/etc/


drcom.conf换三个参数
一、账号
二、密码
三、mac（使用工具上随机生成）

