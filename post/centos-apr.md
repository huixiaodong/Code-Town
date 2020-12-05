

# Docker安装APR



- 安装jdk。

安装时一定选择Oracle的jdk，不能使用openjdk。


- 安装依赖：

```
yum install apr-devel openssl-devel
```

- 进入native目录执行：

```
./configure
make
make install
```

- Tomcat中 catalina.sh配置

```
JAVA_OPTS="$JAVA_OPTS -Djava.library.path=/usr/local/apr/lib"
```

- 文档地址：

http://tomcat.apache.org/native-doc/


###### [返回首页](../) 