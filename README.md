# docker
Under IIEC-RISE 1.0 Campaign I learnt about Docker under the guidance of Vimal Daga Sir. 
This is my final project using Docker
Pre-configurations needed:

I am using RedHat Enterprise Linux. Plus I have also installed Docker Software in it. You can use any OS and inside that OS you should have docker software installed. There might be a possibility that some Linux command might be different from other OS but I will explain what is the work of that command.

1 Pulling MySQL Image:
Use docker pull mysql:5.6 to download the mysql version 5.6 image to use as a database server.
To know more about MySQL Image go to this page: https://hub.docker.com/_/mysql

2 Pulling Wordpress Image:
Use docker pull Wordpress:3.9-php7.2-apache to download the wordpress Image in which php and apache server is already preconfigured.


To know more about Joomla Image go to this page: https://hub.docker.com/_/wordpress
Setting up MySQL:
Use docker run -it -e MYSQL_ROOT_PASSWORD=(any password you like) -e MYSQL_USER=(any user name) -e MYSQL_PASSWORD=(any password(recommended not to use root password) -e MYSQL_DATABASE=(any database name) --name wordpress mysql:5.6 this code and it will create a user with a database inside Your MySQL Server.
