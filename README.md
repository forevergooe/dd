★Linux下网络安装Debian/Ubuntu/CentOS/Windows纯净版一键脚本

仅适用于KVM，不适合OpenVZ。

默认root密码为 MoeClub.org

1、Debian/Ubuntu:

apt-get update

apt-get install -y xz-utils openssl gawk file


apt-get install wget


2、RedHat/CentOS:

yum update

yum install -y xz openssl gawk file


yum -y install wget


★萌咖

默认root密码为 MoeClub.org


1、Debian 9 64位：

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/forevergooe/dd/master/InstallNET.sh') -d 9 -v 64 -a


2、CentOS 6.9 64位：

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/forevergooe/dd/master/InstallNET.sh') -c 6.9 -v 64 -a


★cxthhhhh [魔改版]一键网络重装系统

默认密码是 cxthhhhh.com

wget -N --no-check-certificate "https://raw.githubusercontent.com/forevergooe/dd/master/Network-Reinstall-System-Modify.sh" && chmod a+x Network-Reinstall-System-Modify.sh


1、Debian 9 64位

bash Network-Reinstall-System-Modify.sh -Debian_9

2、CentOS 6.9 64位：

bash Network-Reinstall-System-Modify.sh -CentOS_6

3、CentOS 7 64位：

bash Network-Reinstall-System-Modify.sh -CentOS_7



★综合脚本


wget -N --no-check-certificate "https://raw.githubusercontent.com/forevergooe/dd/master/AutoReinstall.sh" && chmod a+x AutoReinstall.sh && bash AutoReinstall.sh



★CentOS 7 64位安装


1、dansnow              CentOS 7的root密码为 Pwd@CentOS

wget --no-check-certificate -qO AutoDD.sh 'https://raw.githubusercontent.com/forevergooe/dd/master/autodd.sh' && bash AutoDD.sh


2、cxthhhhh.com      CentOS 7的root密码 cxthhhhh.com

wget --no-check-certificate -qO AutoDDT.sh 'https://raw.githubusercontent.com/forevergooe/dd/autoddt.sh' && bash AutoDDT.sh


★Linux镜像源

http://mirrors.aliyun.com/debian/

http://mirrors.163.com/debian/

http://ftp.debian.org/debian/

http://mirrors.edge.kernel.org/debian/

http://ftp.hk.debian.org/debian/

http://ftp.us.debian.org/debian/

http://ftp.jp.debian.org/debian/

http://ftp.ru.debian.org/debian/

http://mirrors.tuna.tsinghua.edu.cn/centos-vault/



