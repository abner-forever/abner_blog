### Linux操作系统安装Nginx (centos7.x)

##### 1. 在终端的任意目录下 安装依赖

 ```
yum install gcc
 ```

```
yum install pcre-devel
```

```
yum install zlib zlib-devel
```

```
yum install openssl openssl-devel
```

##### 2 . 下载nginx tar包

> 创建文件夹

```
cd /usr/local
```

```
mkdir nginx
```

```
cd nginx 
```

> 在此目录下下载包

```
wget http://nginx.org/download/nginx-1.13.7.tar.gz
```

> 解压

```
tar -xvf nginx-1.13.7.tar.gz
```

##### 3.安装nginx

> 进入刚才解压的文件目录

```
cd  nginx-1.13.7
```

> 在此目录下执行命令

```
./configure
```

>  执行make命令

```
make
```

> 执行make install

```
make install
```

##### 4. 测试是否安装成功

```
cd /usr/local/nginx

//在此目录下可以查看安装目录里面的文件

进入sbin目录
cd sibn
执行命令
./nginx -t
```

![执行成功显示图样](\images\QQ截图20181216134404.png)

如上图显示说明成功 

执行./nginx 启动nginx 服务器 就ok了
