# debian

## 介绍

> The universal operating system

## 收录版本

* sid (unstable)
* buster (10 testing)
* stretch (9 stable)
* jessie (8 oldstable)
* wheezy (7 oldoldstable)

## 收录架构

* x86_64
* i386
* armhf

*注：未收录 kfreebsd 和 hurd*

## 使用说明

以`stretch`为例，编辑`/etc/apt/sources.list`, 在文件最前面添加以下条目(操作前请做好相应备份)

```
deb http://mirrors.xdlinux.info/debian/ stretch main non-free contrib
deb-src http://mirrors.xdlinux.info/debian/ stretch main non-free contrib

deb http://mirrors.xdlinux.info/debian/ stretch-proposed-updates main non-free contrib
deb-src http://mirrors.xdlinux.info/debian/ stretch-proposed-updates main non-free contrib
```

安全更新请参见 [debian-security](./debian-security.md)  
*注：testing 和 unstable 不提供安全更新*

## 相关链接

* 官方主页: [https://www.debian.org/](https://www.debian.org)
* 邮件列表: [https://www.debian.org/support#mail_lists](https://www.debian.org/support#mail_lists)
* Wiki: [https://wiki.debian.org/](https://wiki.debian.org/)
* 文档: [https://www.debian.org/doc/](https://www.debian.org/doc/)
* 镜像列表: [https://www.debian.org/mirror/list](https://www.debian.org/mirror/list)
