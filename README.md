# 89xdf

####English Manual
#####Checkout PHP doc tree

````
 $ mkdir /tmp/svn
 $ cd /tmp/svn
 $ svn co https://svn.php.net/repository/phpdoc/modules/doc-en doc-en
 $ cd /tmp/svn/doc-en
````

- 2013.12.19  
	加入PHPExcel  
	Tools添加向浏览器返回文件的函数  
- 2013.12.05  
	加入命令行请求入口，请求示例：`php -f indexc.php "request_uri=/crontab/crontab/index"`  
	增加module的示例代码，包括后台及命令行，在模块的controllers同级目录建立views文件夹，模板文件放置及命名规则同APPLICATION_DIR/views文件夹  
- 2013.10.14  
	格式化framework的代码，修复了framework的一处可能导致redeclare class的错误  
- 2013.10.04  
	加入了[yaf_phpport](https://github.com/mzsolti/yaf-phpport)，方便使用虚拟空间的用户使用yaf框架  

【功能说明】
- 缓存：APC/文件/Memcache/Xcache 源自 [prestashop](https://github.com/PrestaShop/PrestaShop)
- 数据库：MYSQLi/PDO/MYSQL 源自 [prestashop](https://github.com/PrestaShop/PrestaShop) ，可以通过配置mysql_cache_enable控制是否cache查询结果
- 邮件支持：PHPMailer+Vemplator，可以通过建立模板文件，用Vemplator渲染后发送邮件
- 淘宝SDK：Taobao/*，将淘宝公布的SDK按照Yaf加载规则稍作了修改
- Smarty：流行好用的视图引擎
- Blowfish/Rijndael：加解密算法


#####Yaf doc

Yaf documents could be found under doc-en/en/reference/yaf

#####Build Yaf doc

````
$ /path-to-php/bin/php -n -d memory_limit=2G doc-base/configure.php --with-php=/path-to-php/bin/php --enable-xml-details
$ /path-to-ph/bin/phd -d doc-base/.manual.xml --format=php --package=PHP --partial=book.yaf
````

if no errros are reported, then you can find the output under doc-en/output

####Chinese Manual


