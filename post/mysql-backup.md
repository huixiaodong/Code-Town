
# Mysql备份

- 创建用户名密码文件

```
mysql_config_editor set --login-path=local --host=localhost --user=root --password
```

- 使用mysqlpump:
```
/mysql/mysql/bin/mysqlpump --login-path=local dknow | gzip > /mysql/backup/dknow_$(date +%Y%m%d%H%M).sql.gz
```


###### [返回首页](../) 