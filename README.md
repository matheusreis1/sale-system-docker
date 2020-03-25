# sale-system-docker
Docker enviroment to use sale-system repository.

## How to use

- First, you need to clone sale-system repository to app/ folder.
```
cd app/
git clone https://github.com/matheusreis1/sale-system.git
```

- Then, change MySQL configuration in config/config.php
```
define('DB_USER' ,$_ENV['MYSQL_USER']);

define('DB_PASSWORD', $_ENV['MYSQL_PASS']);

define('DB_HOST', 'mysql');
```
