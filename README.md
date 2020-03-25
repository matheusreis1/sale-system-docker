# sale-system-docker
Docker enviroment to use sale-system repository.

## How to use
! Make sure your port 80 is free to use

- Clone this repository
```
git clone https://github.com/matheusreis1/sale-system-docker.git
```

- Then, you need to clone sale-system repository to app/ folder.
```
git clone https://github.com/matheusreis1/sale-system.git app/sale-system/
```

- Then, change MySQL configuration in app/sale-system/config/config.php
```
define('DB_USER' ,$_ENV['MYSQL_USER']);

define('DB_PASSWORD', $_ENV['MYSQL_PASS']);

define('DB_HOST', 'mysql');
```

- Back to sale-system-docker folder, run
```
docker-compose up -d --build
```

- Access in your browser:
http://localhost/sale-system/public/
