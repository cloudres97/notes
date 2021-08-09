## V2Ray配置（Ubuntu|Debian）

##### 1.时间同步

​	服务器与客户端不要求时区一致

```sh
$ date -R	//查看时间
```

##### 2.脚本安装

```sh
$ apt update
```

```sh
$ apt install curl
```

下载安装脚本

```sh
$ curl -O https://raw.githubusercontent.com/v2fly/fhs-install-v2ray/master/install-release.sh
```

执行安装|升级

```sh
$ bash install-release.sh
```

运行

```sh
$ systemctl start v2ray
```

设置开机自启动

```sh
$ systemctl enable v2ray
```

查看是否成功运行

```sh
$ systemctl status v2ray
```

关闭 *v2ray​*

```sh
$ systemctl stop v2ray
```

##### 3.配置 *VMess*

*注意v2ray配置文件在 */usr/local/etc/v2ray* 下

