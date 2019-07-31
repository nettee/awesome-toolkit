# 网络

## Nginx

### 配置文件

Nginx 有几种配置文件：

+ `sites-available` 通常写配置的地方
+ `sites-enabled` 生效的配置，放符号链接，指向 `sites-available` 中的内容
+ `nginx.conf` 总的配置文件，在最后 include 了 `sites-enabled` 中的内容

参考：

+ 查看 nginx 配置文件位置：[如何找出nginx配置文件的所在位置？](https://juejin.im/entry/5a9ce1c06fb9a028e11f70f2)


## Privoxy 将SOCKS5代理转换为HTTP代理

```Bash
sudo vim /etc/privoxy/config
```

插入一行
```
forward-socks5    /    127.0.0.1:1080     .
```

注意：不要忘记最后那一个点！

```Bash
sudo service privoxy restart
```
