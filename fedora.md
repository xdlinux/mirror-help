# fedora

## 介绍

> Fedora Workstation is a polished, easy to use operating system for laptop and desktop computers, with a complete set of tools for developers and makers of all kinds.

> Fedora Server is a powerful, flexible operating system that includes the best and latest datacenter technologies. It puts you in control of all your infrastructure and services.

> Fedora Atomic provides the best platform for your Linux-Docker-Kubernetes (LDK) application stack.

## 收录版本

* 26
* 25

## 收录架构

* x86_64
* i386

## 使用说明

将以下保存为 `fedora-xdlinux.repo`

```
[fedora]
name=Fedora $releasever - $basearch - xdlinux
failovermethod=priority
baseurl=https://mirrors.xdlinux.info/fedora/releases/$releasever/Everything/$basearch/os/
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=fedora-$releasever&arch=$basearch
enabled=1
metadata_expire=7d
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$basearch

[fedora-debuginfo]
name=Fedora $releasever - $basearch - Debug - xdlinux
failovermethod=priority
baseurl=https://mirrors.xdlinux.info/fedora/releases/$releasever/Everything/$basearch/debug/
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=fedora-debug-$releasever&arch=$basearch
enabled=0
metadata_expire=7d
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$basearch

[fedora-source]
name=Fedora $releasever - Source - xdlinux
failovermethod=priority
baseurl=https://mirrors.xdlinux.info/fedora/releases/$releasever/Everything/source/SRPMS/
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=fedora-source-$releasever&arch=$basearch
enabled=0
metadata_expire=7d
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$basearch
```

将以下保存为 `fedora-updates-xdlinux.repo`

```
[updates]
name=Fedora $releasever - $basearch - Updates - xdlinux
failovermethod=priority
baseurl=https://mirrors.xdlinux.info/fedora/updates/$releasever/$basearch/
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=updates-released-f$releasever&arch=$basearch
enabled=1
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$basearch

[updates-debuginfo]
name=Fedora $releasever - $basearch - Updates - Debug -xdlinux
failovermethod=priority
baseurl=https://mirrors.xdlinux.info/fedora/updates/$releasever/$basearch/debug/
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=updates-released-debug-f$releasever&arch=$basearch
enabled=0
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$basearch

[updates-source]
name=Fedora $releasever - Updates Source - xdlinux
failovermethod=priority
baseurl=https://mirrors.xdlinux.info/fedora/updates/$releasever/SRPMS/
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=updates-released-source-f$releasever&arch=$basearch
enabled=0
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$basearch
```

先备份 `/etc/yum.repos.d/fedora.repo` 和 `/etc/yum.repos.d/fedora-updates.repo`

将 `fedora-xdlinux.repo` 和 `fedora-updates-xdlinux.repo` 放入 `/etc/yum.repos.d/` 中.

运行：

```
sudo dnf makecache
```

## 相关链接

* 官方主页: [https://getfedora.org/](https://getfedora.org/)
* 邮件列表: [https://fedoraproject.org/wiki/Communicate](https://fedoraproject.org/wiki/Communicate)
* 论坛: [https://forums.fedoraforum.org/](https://forums.fedoraforum.org/)
* Wiki: [https://fedoraproject.org/wiki/](https://fedoraproject.org/wiki/)
* 文档: [https://docs.fedoraproject.org/](https://docs.fedoraproject.org/)
