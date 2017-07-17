# CentOS

## 介绍

> The CentOS Project is a community-driven free software effort focused on delivering a robust open source ecosystem.

## 收录版本

* 7
* 6

## 收录架构

* x86_64
* i386

## 使用说明


首先备份 `CentOS-Base.repo`

```
mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo.backup
```

以 `CentOS 7` 为例， 编辑 `/etc/yum.repos.d/CentOS-Base.repo`

```
# CentOS-Base.repo
#
# The mirror system uses the connecting IP address of the client and the
# update status of each mirror to pick mirrors that are updated to and
# geographically close to the client.  You should use this for CentOS updates
# unless you are manually picking other mirrors.
#
# If the mirrorlist= does not work for you, as a fall back you can try the
# remarked out baseurl= line instead.
#
#

[base]
name=CentOS-$releasever - Base
#mirrorlist=http://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=os
baseurl=https://mirrors.xdlinux.info/centos/$releasever/os/$basearch/
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7

#released updates
[updates]
name=CentOS-$releasever - Updates
# mirrorlist=http://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=updates
baseurl=https://mirrors.xdlinux.info/centos/$releasever/updates/$basearch/
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7

#additional packages that may be useful
[extras]
name=CentOS-$releasever - Extras
# mirrorlist=http://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=extras
baseurl=https://mirrors.xdlinux.info/centos/$releasever/extras/$basearch/
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7

#additional packages that extend functionality of existing packages
[centosplus]
name=CentOS-$releasever - Plus
# mirrorlist=http://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=centosplus
baseurl=https://mirrors.xdlinux.info/centos/$releasever/centosplus/$basearch/
gpgcheck=1
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
```

运行 `sudo yum makecache` 生成缓存.

## 相关链接

* 官方主页: [https://www.centos.org/](https://www.centos.org/)
* 邮件列表: [https://www.centos.org/modules/tinycontent/index.php?id=16](https://www.centos.org/modules/tinycontent/index.php?id=16)
* 论坛: [https://www.centos.org/modules/newbb/](https://www.centos.org/modules/newbb/)
* 文档: [https://www.centos.org/doc/](https://www.centos.org/doc/)
* Wiki: [https://wiki.centos.org/](https://wiki.centos.org/)
* 镜像列表: [https://www.centos.org/modules/tinycontent/index.php?id=32](https://www.centos.org/modules/tinycontent/index.php?id=32)
