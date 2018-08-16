# Oracal-安装教程
root用户登录虚拟机
+ 修改主机名
```
hostnamectl set-hostname oracle01
```
```
vi /etc/hosts 
```
添加如下行
```
localhost  oracle01
```
+ 修改selinux模式为disabled
```
vi /etc/selinux/config
```
```
SELINUX=disabled
```
+ 新建一个目录software（权限为777）
```
mkdir software
chmod 777 software
```
+ 安装如下安装包
```
yum install binutils-2.27-28.base.el7_5.1 compat-libstdc++-33-3.2.3-72.el7 elfutils-libelf-devel-0.170-4.el7 glibc-devel-2.17-222.el7 gcc-4.8.5-28.el7_5.1 gcc-c++-4.8.5-28.el7_5.1  libaio-devel-0.3.109-13.el7 libgcc-4.8.5-28.el7_5.1.x86_64 libstdc++-4.8.5-28.el7_5.1 libstdc++-devel-4.8.5-28.el7_5.1 make-3.82-23.el7.x86_64 sysstat-10.1.5-13.el7.x86_64 unixODBC-2.3.1-11.el7 unixODBC-devel-2.3.1-11.el7 libXp-1.0.2-2.1.el7
```
