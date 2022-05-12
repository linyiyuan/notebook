1. Mac安装Swoole提示ssld相关错误，需要手动指定openssl目录

```php
./configure --enable-openssl --with-openssl-dir=/usr/local/opt/openssl --enable-http2 --with-php-config=/Applications/MxSrvs/bin/php/bin/php-config

```

2. Hyperf使用Cos腾讯云上传超过1M大小的图片时报Curl相关错误，可能是由于`Swoole` 安装时没有指定Curl, 在安装swolle的时候手动指定开启curl即可

```php
./configure --with-php-config=/usr/local/php/bin/php-config --enable-swoole-curl
```
