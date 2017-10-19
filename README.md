# You need a webserver for develop
Install step by step webserver on ubuntu 16.04 LTS

## dev@north-d:~$ apt-get -y install mysql-server mysql-client
## dev@north-d:~$ mysql_secure_installation
## dev@north-d:~$ mysql -u root -p
## dev@north-d:~$ sudo apt -y install phpmyadmin
## dev@north-d:~$ sudo apt -y install php7.0 libapache2-mod-php7.0
## dev@north-d:~$ systemctl restart apache2
## dev@north-d:~$ nano /var/www/html/info.php
## dev@north-d:~$ sudo chown www-data:www-data /var/www/html/info.php
## dev@north-d:~$ apt-cache search php7.0
## dev@north-d:~$ sudo apt -y install php7.0-mysql php7.0-curl php7.0-gd php7.0-intl php-pear php-imagick php7.0-imap php7.0-mcrypt php-memcache php7.0-pspell php7.0-recode php7.0-sqlite3 php7.0-tidy php7.0-xmlrpc php7.0-xsl php7.0-mbstring php-gettext
## dev@north-d:~$ sudo apt -y install php7.0-opcache php-apcu
## dev@north-d:~$ systemctl restart apache2
## dev@north-d:~$ sudo a2enmod ssl
## dev@north-d:~$ sudo a2ensite default-ssl.conf
## dev@north-d:~$ systemctl restart apache2 
done

sumber: https://www.howtoforge.com/tutorial/install-apache-with-php-and-mysql-on-ubuntu-16-04-lamp/
