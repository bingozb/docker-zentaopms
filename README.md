# docker-zentaopms
Docker image for ZenTao project management software. （禅道开源版 11.5.1 2019-06-25）

![宏狼科技PMS](https://raw.githubusercontent.com/bingozb/docker-zentaopms/master/demo.png)

## 说明
本镜像基于禅道源代码进行安装，镜像中已经安装 `Nginx` 1.13.9、`PHP` 5.6-fpm 以及禅道依赖的 `pdo`、` pdo_mysql`、`json`、`filter`、`openssl`、`mbstring`、`zlib`、`curl`、`gd`、`iconv` 这些模块。

![系统扩展检查](https://raw.githubusercontent.com/bingozb/docker-zentaopms/master/vendor.png)

## 关于数据库
本镜像不包含数据库，个人觉得数据库比较重要，请自行另外搭建或采用成熟稳定的云数据库服务。如果要自行搭建，建议运行一个容器来单独运行数据库服务，而不是基于这个镜像把数据库服务也装到一起。另外，官方建议是使用 MYSQL 5.5 / 5.6，亲测 5.7 也可以正常使用。

## 相关
https://www.zentao.net
