# 自己的学习笔记 for macOS

## https://panjiachen.github.io/vue-element-admin-site/zh/guide/#%E5%AE%89%E8%A3%85
```shell
## 
## 
$ npm config get registry
https://registry.npmjs.org/
## 
npm install --registry=https://registry.npmmirror.com
## 
## 
go get xorm.io/xorm@v1.3.6
## 
## admin admin@163.com 123456
http://localhost:8088/install
## 
http://localhost:8088/admin
## 
## 
```

```shell
## docker for MySQL8.x
docker run --name studygolang-db-mysql -e MYSQL_ROOT_PASSWORD=123456 \
    -p 3380:3306 \
    -d mysql:8.0.35 \
    --character-set-server=utf8mb4 \
    --collation-server=utf8mb4_unicode_ci \
    --default-authentication-plugin=mysql_native_password
## 
## 
go mod tidy
go work use .
make build
make start
## 
## 在浏览器中输入：http://127.0.0.1:8088
应该就能看到了。

接下来你会看到图形化安装界面，一步步照做吧。

如果之后有出现页面空白，请查看 error.log 是否有错误
## 
## 
## 
going@ubuntu2204 [08:47:57 PM] [~/workspace/golang/src/github.com/godev2009/studygolang] [study]
-> % mysql -hlocalhost -uroot -p123456 -P 3380
## 
MySQL [(none)]> create database studygolang charset utf8mb4 collate utf8mb4_unicode_ci;
Query OK, 1 row affected (0.005 sec)
## 
## 
MySQL [(none)]> use studygolang;
MySQL [(none)]> source config/db.sql;
MySQL [(none)]> source config/init.sql;
## 
```