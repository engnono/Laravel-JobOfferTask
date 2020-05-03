### Laravel Job Offer Project

Installation

> Requires Composer and php7.*

- Create a new MySql Database with charset UTF8mb4 (IMPORTANT)
> use phpmyadmin if you have it connected to your MySql/MariaDB host, or follow the following approach
```
# Connect to Mysql, if host is not on the same machine, add the host flag like this -h <ip_orHostName>
mysql -u <mysql username> -p

# After successful login you will have the mysql or mariadb terminal access
mysql> create database <database_name> character set UTF8mb4 collate utf8mb4_unicode_ci;
```

- Update the .env file with your db credentials
- Run: composer install
- Change storage and cache folders permissions to 777
```
$ chmod 777 -R bootstrap/cache/
$ chmod 777 -R storage/
```
- Change MAIL_MAILER To log in your .env file and APP_URL=http://localhost:8000 if you are using artisan serve
- Run: php artisan serve
