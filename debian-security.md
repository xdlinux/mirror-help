# debian-security

## 使用说明

以`stretch`为例，编辑`/etc/apt/sources.list`, 在文件最前面添加以下条目(操作前请做好相应备份)

```
deb http://mirrors.xdlinux.info/debian-security/ stretch/updates main contrib non-free
deb-src http://mirrors.xdlinux.info/debian-security/ stretch/updates main contrib non-free
```

## 相关链接

见 [debian](./debian.md)
