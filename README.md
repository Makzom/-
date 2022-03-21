annotation：explorer.exe是Windows程序管理器或者文件资源管理器，它用于管理Windows图形壳，包括桌面和文件管理，删除该程序会导致Windows图形界面无法使用


解决方式：把图标缓存的数据库删除

 
第一步：win+r  cmd进入命令行

第二步：一行一行键入如下命令
taskkill /im explorer.exe /f

cd /d %userprofile%\appdata\local

del iconcache.db /a

start explorer.exe

exit

还是不行就找到文件原来位置的exe发送到桌面快捷方式
————————————————
版权声明：本文为CSDN博主「齐木楠隼」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/first52hz/article/details/84969753
