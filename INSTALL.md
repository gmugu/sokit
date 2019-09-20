# 编译运行方法
本文档INSTALL.md描述如何安装并配置开发环境(主要是安装Qt5和QtCreator)

## 编译步骤
1. Ubuntu命令行执行`sudo apt install qtcreator qt5-default qtbase5-dev qttools5-dev`安装开发环境；
2. 安装成功后打开Ubuntu左下角开始菜单，找到QtCreator并运行；
3. 打开项目子目录内的工程文件build/general/qtcreator/sokit.pro；
4. 按照QtCreator主窗口的提示，对工程进行初始配置，勾选Select all kits然后点击Configure Project；
5. 点击左下方的三角形开始编译，编译耗时较长，耐心等待几分钟，编译成功后开始运行本程序。

## 编译输出
编译输出目录位于项目的bin/debug(或release)子文件夹下
 - sokit是主程序
 - sokit.lan是Qt中文界面翻译，应与主程序放在同一个目录内。

# 运行依赖库
图形界面是基于Qt5设计的，所以在Ubuntu18.04下运行的话推荐安装qt5-default：

    sudo apt-get install qt5-default

# 支持的Qt版本
Qt5版本比较多，目前已经测试过的版本如下：
 - Ubuntu 18.04 软件源中的Qt版本为5.9.5；
 - Ubuntu 19.04 已更新至Qt5.12.2；

其他Linux操作系统建议查询各自软件源是否提供的QtCreator的rpm或deb安装包。如果找不到，就去www.qt.io官网下载完整版Qt开发环境，网址如下：
https://www.qt.io/offline-installers
注意官网要求通过email邮箱方式注册一个帐号才能下载和安装。
