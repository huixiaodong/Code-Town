
# CentOS挂载本地镜像

- 挂载cd：

```
mount /dev/cdrom /media/CentOS
```

- 挂载iso

```
mount -t iso9660 -o loop /usr/local/src/CentOS-7.iso /media/CentOS
```

- 修改本地源：

```
/etc/yum.repo.d/Centos7-Media.repo 的 enable=1
```

- Centos7-Base.repo改为其他名字。
- yum makecache


###### [返回首页](../) 