# deb-multimedia

## 介绍

Debian 第三方多媒体软件源

## 收录版本

* sid (unstable)
* buster (10 testing)
* stretch (9 stable)
* jessie (8 oldstable)
* wheezy (7 oldoldstable)

## 收录架构

* amd64
* i386

*注：未收录 kfreebsd 和 hurd*

## 使用说明

以 `stretch` 为例，编辑 `/etc/apt/sources.list` 文件，在文件开头添加以下内容  
请根据需要去掉 `deb-src` 和 `backports` 前面的注释

```
deb http://mirrors.xdlinux.info/debian-multimedia/ stretch main contrib non-free
#deb-src http://mirrors.xdlinux.info/debian-multimedia/ stretch main contrib non-free

#deb http://mirrors.xdlinux.info/debian-multimedia/ stretch-backports main contrib non-free
#deb-src http://mirrors.xdlinux.info/debian-multimedia/ stretch-backports main contrib non-free
```

## 相关链接

* 官方主页: [https://deb-multimedia.org/](https://deb-multimedia.org/)
* 邮件列表: [https://deb-multimedia.org/mailinglist](https://deb-multimedia.org/mailinglist)
* 镜像列表: [https://deb-multimedia.org/deb-m](https://deb-multimedia.org/deb-m)
