# epel

## 介绍

EPEL (Extra Packages for Enterprise Linux) ，适用于 Red Hat Enterprise Linux (RHEL)， CentOS， Scientific Linux (SL)， Oracle Linux (OL)

## 收录版本

* 6
* 7

## 收录架构

* i386
* x86_64

## 使用说明

若存在则先备份 `/etc/yum.repos.d/epel.repo` 和 `/etc/yum.repos.d/epel-testing.repo`  
以版本 `7` 为例，复制以下内容到 `/etc/yum.repos.d/epel.repo`

```
[epel]
name=Extra Packages for Enterprise Linux 7 - $basearch
baseurl=http://mirrors.xdlinux.info/epel/7/$basearch
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-7&arch=$basearch
failovermethod=priority
enabled=1
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7

[epel-debuginfo]
name=Extra Packages for Enterprise Linux 7 - $basearch - Debug
baseurl=http://mirrors.xdlinux.info/epel/7/$basearch/debug
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-debug-7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1

[epel-source]
name=Extra Packages for Enterprise Linux 7 - $basearch - Source
baseurl=http://mirrors.xdlinux.info/epel/7/SRPMS
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-source-7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1
epel-testing.repo

[epel-testing]
name=Extra Packages for Enterprise Linux 7 - Testing - $basearch
baseurl=http://mirrors.xdlinux.info/epel/testing/7/$basearch
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-epel7&arch=$basearch
failovermethod=priority
enabled=0
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7

[epel-testing-debuginfo]
name=Extra Packages for Enterprise Linux 7 - Testing - $basearch - Debug
baseurl=http://mirrors.xdlinux.info/epel/testing/7/$basearch/debug
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-debug-epel7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1

[epel-testing-source]
name=Extra Packages for Enterprise Linux 7 - Testing - $basearch - Source
baseurl=http://mirrors.xdlinux.info/epel/testing/7/SRPMS
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-source-epel7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1
```

运行 `sudo yum makecache` 生成缓存

## 相关链接

* Wiki: [http://fedoraproject.org/wiki/EPEL](http://fedoraproject.org/wiki/EPEL)
* FAQ: [http://fedoraproject.org/wiki/EPEL/faq](http://fedoraproject.org/wiki/EPEL/faq)
