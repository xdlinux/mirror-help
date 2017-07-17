# Ubuntu

## 介绍

> Ubuntu is an open source software platform that runs from the cloud, to the smartphone, to all your things

## 收录版本

* artful (17.10)
* zesty (17.04)
* yakkety (16.10)
* xenial (16.04 LTS)
* wily (15.10)
* trusty (14.04 LTS)
* precise (12.04 LTS)

## 收录架构

* amd64
* i386

## 使用说明

以`xenial`为例，编辑`/etc/apt/sources.list`， 在文件开头添加以下内容
请根据需要去掉 `deb-src` 以及 `proposed-updates` 和 `backports` 前面的注释

```
deb http://mirrors.xdlinux.info/ubuntu/ xenial main restricted universe multiverse
#deb-src http://mirrors.xdlinux.info/ubuntu/ xenial main restricted universe multiverse

deb http://mirrors.xdlinux.info/ubuntu/ xenial-security main restricted universe multiverse
#deb-src http://mirrors.xdlinux.info/ubuntu/ xenial-security main restricted universe multiverse

deb http://mirrors.xdlinux.info/ubuntu/ xenial-updates main restricted universe multiverse
#deb-src http://mirrors.xdlinux.info/ubuntu/ xenial-updates main restricted universe multiverse

#deb http://mirrors.xdlinux.info/ubuntu/ xenial-backports main restricted universe multiverse
#deb-src http://mirrors.xdlinux.info/ubuntu/ xenial-backports main restricted universe multiverse

#deb http://mirrors.xdlinux.info/ubuntu/ xenial-proposed main restricted universe multiverse
#deb-src http://mirrors.xdlinux.info/ubuntu/ xenial-proposed main restricted universe multiverse
```

## 相关链接

* 官方主页: [https://www.ubuntu.com/](https://www.ubuntu.com/)
* 邮件列表: [https://www.ubuntu.com/support/community/mailinglists](https://www.ubuntu.com/support/community/mailinglists)
* 论坛: [https://ubuntuforums.org/](https://ubuntuforums.org/)
* 中文论坛: [https://forum.ubuntu.org.cn/](https://forum.ubuntu.org.cn/)
* Wiki: [httpss://wiki.ubuntu.com/](httpss://wiki.ubuntu.com/)
* 文档: [httpss://help.ubuntu.com/](httpss://help.ubuntu.com/)
