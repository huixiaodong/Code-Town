
# SELINUX

- 查看状态

```
/usr/sbin/sestatus -v 

或

getenforce
```

- 关闭SELINUX:


临时：

```
setenforce 0 ##设置 SELinux 成为 permissive 模式

##setenforce 1 设置 SELinux 成为 enforcing 模式
```

永久：

vi /etc/selinux/config
将 SELINUX=enforcing 改为 SELINUX=disabled
重启机器即可


###### [返回首页](../) 