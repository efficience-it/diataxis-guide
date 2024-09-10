# First Installation

For docker installation
```bash
  docker compose build
  docker compose up -d
```


Installation des vendors et des assets de nelmio
```bash
  docker exec php-fpm composer install
  docker exec php-fpm php bin/console assets:install
```

Dump an .env file as the .env.local.php
```bash
  docker exec php-fpm composer dump-env dev
```

## local hosts to set
- on windows: C:\Windows\System32\drivers\etc\hosts
- on linux, mac: /etc/hosts

Add this line:
```
127.0.0.1 diataxis.localhost
```
