
## Rodando PHP com Debug

docker compose -f docker/docker-compose.yml up --build -d




*Php MyAdmin*

localhost:8080

*php*

localhost:8081

*Loggin*

Os logs do nginx são gerados em logs

*MariaDB*

user:root

pass:root



volumes:
            - ../public:/var/www/html
            - ../php/conf.d/90-xdebug.ini:/usr/local/etc/php/conf.d/90-xdebug.ini
            - ../php/conf.d/error_reporting.ini:/usr/local/etc/php/conf.d/error_reporting.ini
            - ../php/conf.d/php.ini:/usr/local/etc/php/php.ini
            - ../php/xdebug/log/xdebug-codeigniter.log:/tmp/xdebug/xdebug-codeigniter.log
