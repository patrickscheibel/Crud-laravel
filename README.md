# Instalação das tecnologias utilizadas
## PHP
$ apt install php php-xml php-pgsql

## Composer
$ apt install composer

## Docker Compose(Opcional)
$ apt install docker-compose

# Sistema
## Clone
$ git clone https://gitlab.com/patrick.scheibel/crud-laravel.git

## Depois de baixar o projeto, acesse a pasta e instale as dependências necessárias
$ composer install

Para acessar o banco, crie uma cópia do arquivo .env e configure a conexão.\
Utilizei migration para o banco de dados, mas caso seja necessário, o script com o sql está na pasta <i>database</i>.

## Criar e executar o banco pelo docker-compose(Opcional)
$ docker-compose up -d

## Executar as migrations(Opcional)
$ php artisan migrate

## Gerar chave necessária para executar o sistema
$ php artisan key:generate

## Executar o sistema 
$ php artisan serve
