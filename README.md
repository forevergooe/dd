# dd
Linux下网络安装Debian/Ubuntu/CentOS/Windows纯净版一键脚本
仅适用于KVM，不适合OpenVZ。
默认root密码为 MoeClub.org

一、安装软件
Debian/Ubuntu:
apt-get update
apt-get install -y xz-utils openssl gawk file

RedHat/CentOS:
yum update
yum install -y xz openssl gawk file

二、下载脚本
wget --no-check-certificate https://zhujiwiki.com/wp-content/uploads/2018/04/InstallNET.sh
chmod -x InstallNET.sh

三、安装系统
（一）安装Debian各版本
1、安装Debian 7 x32
bash InstallNET.sh -d 7 -v 32 -a

2、安装Debian 7 x64
bash InstallNET.sh -d 7 -v 64 -a

3、安装Debian 8 x32
bash InstallNET.sh -d 8 -v 32 -a

4、安装Debian 8 x64
bash InstallNET.sh -d 8 -v 64 -a

5、安装Debian 9 x32
bash InstallNET.sh -d 9 -v 32 -a

6、安装Debian 9 x64
bash InstallNET.sh -d 9 -v 64 -a

（二）安装Ubuntu各版本
1、安装Ubuntu 14.04 x32
bash InstallNET.sh -u trusty -v 32 -a

2、安装Ubuntu 14.04 x64
bash InstallNET.sh -u trusty -v 64 -a

3、安装Ubuntu 16.04 x32
bash InstallNET.sh -u xenial -v 32 -a

4、安装Ubuntu 16.04 x64
bash InstallNET.sh -u xenial -v 64 -a

5、安装Ubuntu 17.04 x32
bash InstallNET.sh -u zesty -v 32 -a

6、安装Ubuntu 17.04 x64
bash InstallNET.sh -u zesty -v 64 -a

（三）安装CentOS各版本
1、安装CentOS 6.8 32位
bash InstallNET.sh -c 6.8 -v 32 -a --mirror 'http://vault.centos.org'

2、安装CentOS 6.8 64位
bash InstallNET.sh -c 6.8 -v 64 -a --mirror 'http://vault.centos.org'

3、安装CentOS 6.9 32位
bash InstallNET.sh -c 6.9 -v 32 -a --mirror 'http://vault.centos.org'

4、安装CentOS 6.9 64位
bash InstallNET.sh -c 6.9 -v 64 -a --mirror 'http://vault.centos.org'

（四）安装Windows Server2012 R2 data center
这个建议在Debian9下DD安装。
bash InstallNET.sh -dd 'https://down.zhujiwiki.com/windows-dd/S2012R2DATA2018410.vhd.gz'

这个版本特点：
原版系统只添加驱动
打包防勒索补丁，在防火墙屏蔽135、137、138、139、445端口
自动开启远程登录（密码需要安装的时候自己设置）
登录取消ctrl alt delete
系统盘默认12G，其他的请使用扩展卷添加

四、使用参数详解
bash InstallNET.sh

-d/--debian [dist-name]
-u/--ubuntu [dist-name]
-c/--centos [dist-version]
-v/--ver [32/i386|64/amd64]
--ip-addr/--ip-gate/--ip-mask
-apt/-yum/--mirror
-dd/--image
-a/-m
# dist-name: 发行版本代号
# dist-version: 发行版本号
# -apt/-yum/--mirror : 使用定义镜像
# -a/-m : 询问是否能进入VNC自行操作. -a 为不提示(一般用于全自动安装), -m 为提示.
