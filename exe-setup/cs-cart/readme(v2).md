FOLOW https://docs.cs-cart.com/latest/install/nginx.html



thay đổi /etc/php.ini:
+ ;cgi.fix_pathinfo=1 -> cgi.fix_pathinfo=0

thay đổi /etc/php-fpm.d/www.conf:
+ listen = 127.0.0.1:9000
+ user = nginx
+ group = nginx
+ listen.owner = nobody
+ listen.group = nobody


cp nginx.conf




https://www.digitalocean.com/community/tutorials/how-to-install-linux-nginx-mysql-php-lemp-stack-on-centos-7
https://docs.cs-cart.com/latest/install/nginx.html
https://www.php.net/manual/en/install.unix.nginx.php
https://linuxize.com/post/install-php-7-on-centos-7/