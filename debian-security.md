# debian-security

## 介绍

debian 的安全更新

## 收录版本

* stretch (9 stable)
* jessie (8 oldstable)
* wheezy (7 oldoldstable)

## 收录架构

* x86_64
* i386

*注：未收录 kfreebsd 和 hurd*

## 使用说明

以`stretch`为例，编辑`/etc/apt/sources.list`, 在文件开头添加以下内容  
请根据需要去掉 `deb-src` 前面的注释

```
deb http://mirrors.xdlinux.info/debian-security/ stretch/updates main contrib non-free
#deb-src http://mirrors.xdlinux.info/debian-security/ stretch/updates main contrib non-free
```

## 相关链接

见 [debian](./debian.md)
