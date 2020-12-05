
# Docker 安装


- docker安装：
```
https://docs.docker.com/install/linux/docker-ce/centos/
```
- docker-compose 安装：
```
https://docs.docker.com/compose/install/
```

- 删除名字是 none 的镜像：
```
docker rmi $(docker images -f  "dangling=true" -q)
```

- 给非 root 用户授权：
```
usermod -aG docker $USER
```
