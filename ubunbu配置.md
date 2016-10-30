###ubunbu 配置
------------

####安装fcitx五笔
`sudo apt install fcitx-table-wubi`

####安装shadowsocks-qt5
`sudo add-apt-repository ppa:hzwhuang/ss-qt5`
`sudo apt update`
`sudo apt install shadowsocks-qt5`

>**配置pac**

>1. 安装pip 
`sudo apt install python-pip`
>2. 安装genpac 
`pip install genpac`  升级 `pip install --upgrade genpac`   卸载  `pip uninstall genpac`
>3. 创建一个目录及文件 
`touch user-rules.txt`
>4. 进入文件夹配置（先登录shadowsocks） 
`genpac -p "SOCKS5 127.0.0.1:1080" --gfwlist-proxy="SOCKS5 127.0.0.1:1080" --output="autoproxy.pac" --gfwlist-url="https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt" --user-rule-from="user-rules.txt"`
>5. 设置全局代理为自动 ， 配置URL选择**autoproxy.pac**文件，应用即可
>格式如：file:///home/{user}/××××/autoproxy.pac 

>**使用finalspeed加速人ss，需要java环境 (客户端配置，服务端略)**

>1. `java -jar finalspeed_client.jar`

>2. 配置finalspeed：设置宽带（正常的60%左右）---> 服务器ss地址 ---> 添加  ---> ss加速端口 ---> 本地端口随意（2000）

>3. 配置ss：服务器地址 127.0.0.1  ---> 服务器端口（2000）---> ss密码 ---> 本地端口默认1080

####[设置英文文件夹](http://jingyan.baidu.com/article/49711c6170cb0afa441b7c1b.html)

####安装文泉字体
`sudo apt-get install ttf-wqy-microhei`

####安装wine

>直接安装：`sudo apt install wine`

>此为新版未能成功安装QQ

>`sudo dpkg --add-architecture i386 `

>`sudo add-apt-repository ppa:wine/wine-builds`

>`sudo apt-get update`

>`sudo apt-get install --install-recommends winehq-devel`

$ winecfg
然后在运行wine

####[安装QQ](http://ttop5.net/?p=1316)


####安装主题美化
1. 安装设置管理工具： 
`sudo apt-get install unity-tweak-tool`
2. 安装Numix主题和图标： 
`sudo add-apt-repository ppa:numix/ppa` 
`sudo apt-get update`   
`sudo apt-get install numix-gtk-theme numix-icon-theme-circle`
3. 增加Arc theme：
`sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/Horst3180/xUbuntu_16.04/ /' >> /etc/apt/sources.list.d/arc-theme.list"`
4. 接收更新的 Arc GTK 主题：
`wget http://download.opensuse.org/repositories/home:Horst3180/xUbuntu_16.04/Release.key`
`sudo apt-key add - < Release.key`
`sudo apt update`
`sudo apt install arc-theme`

####安装vim 、git 、uget下载 、subversion  、wps 、bleachbit清理

####配置ssh
`ssh-keygen`
`vim .ssh/config`	配置Host
`vim .ssh/authorized_keys`	配置authorized_keys

####安装openvpn
`sudo apt install openvpn`

####安装JDK
```
环境变量
export JAVA_HOME=/home/username/jdk1.8.0_111
export CLASSPATH=.:$JAVA_HOME/lib:$JAVA_HOME/jre/lib:$CLASSPATH
export PATH=$JAVA_HOME/bin:$JAVA_HOME/jre/bin:$PATH
```
####安装Android studio
```
adb环境
export PATH=$PATH:/android-sdk-path/tools/
export PATH=$PATH:/android-sdk-path/platform-tools/
```

####安装unar解压（解决解压乱码问题）
`sudo apt install unar`


####删除不用的软件
>libreoffice-common libreoffice
thunderbird 雷鸟邮件客户端
totem 自带的播放器
rhythmbox 自带的音乐播放器
empathy 自带的即时聊天应用
brasero 自带的光盘刻录器
simple-scan 扫描仪
gnome-mahjongg 对对碰游戏
aisleriot 纸牌游戏
gnome-mines 扫雷游戏
cheese webcam 应用
gnome-sudoku 数独游戏
transmission-common BT 客户端
gnome-orca 屏幕阅读
remmina-common
//landscape-client-ui-install landscape 远程控制软件
deja-dup 备份
onboard 屏幕键盘
```
sudo apt purge libreoffice-common
sudo apt purge gnome-orca
```

####[安装云音乐](http://music.163.com/#/download)

####[安装 electronic-wechat](https://github.com/geeeeeeeeek/electronic-wechat/releases)










