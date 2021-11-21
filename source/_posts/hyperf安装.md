#### 安装swoole

选择php7.4版本 

```php
	sudo update-alternatives --config php
```
 
```php
	cd swoole-src-master/
```

```php
	./configure --enable-http2 --enable-openssl --with-php-config=/usr/bin/php-config7.4
	#./configure --with-php-config=/usr/bin/php-config7.4
	# /usr/bin/phpize7.4
```


问题：

如果出现报错： PHP Warning: PHP Startup: Unable to load dynamic library ‘swoole.so’ (tried: /usr/lib/php/20190902/swoole.so (/usr/lib/php/20190902/swoole.so: cannot open shared object file: No such file or directory)

可能是系统存在多个PHP版本，需要指定  --with-php-config=/usr/bin/php-config7.4



相关命令： 

 protoc  ./hello.proto --php_out=/Users/lihongwei/phpcode/hyperf-skeleton/nucarf-grpc/src

