
# Mysql授权


- Mysql授权：

```
create user "username"@"host" identified by "password";

GRANT ALL PRIVILEGES ON hbhy.* TO 'marry'@'%' WITH GRANT OPTION;

FLUSH PRIVILEGES;
```

###### [返回首页](/) 