
# Nginx相关配置


- 从https代理到http，需要在location中添加下列配置：


```
proxy_set_header    X-Forwarded-Proto "https";
proxy_redirect http:// $scheme://;
```

- 代理websocket需要在location添加如下配置：


```
proxy_http_version 1.1;
proxy_set_header Upgrade $http_upgrade;
proxy_set_header Connection "upgrade";
```

- 关闭日志


```
access_log off;
error_log /dev/null;
```

###### [返回首页](../) 