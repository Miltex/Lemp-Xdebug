
# Rodando PHP com Debug

### Esse comando deve ser executado somente a primeira vez.

Clone o repositório e execute os seguinte comandos:

git clone https://github.com/Miltex/Lemp-Xdebug.git .

cd LEMP_STACK_DEBUG 

docker compose -f docker/docker-compose.yml up --build -d



# Acesso ao Public do *php*

localhost:8081

### Geração de Logs - Loggin*

Os logs do nginx são gerados em logs

# Banco de Dados - *MariaDB*

## Acesso ao Database

### Interface com Banco de Dados - *Php MyAdmin*

localhost:8080

Servidor: mariadb

User: root

Pass: root


# Instalação Node no Container

nvm install v21.1.0


# Rodando o Vue JS

### Criando um Projeto com o Vue JS

npm create vue@latest

npm install --silent

npm install --verbose

npm run dev --host=0.0.0.0


# Rodando o Laravel Framework

### Entre no container docker-php com o seguinte comando:

docker exec -it php bash

#### Dentro do container execute os comandos abaixo:

composer create-project laravel/laravel new-app-laravel

php artisan serve --host=0.0.0.0

Acesse o Laravel Framework

http://localhost:8000/