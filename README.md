# InfoProvas API
API/Backend do sistema do InfoProvas, consumida pelos apps e pelo site.

O projeto InfoProvas está sendo atualizado pelo DevMob, com criação de API, Site e App novos.

Tem interesse em participar da nova implementação? Entre em contato conosco por email ou uma de nossas redes sociais. 

Precisa de ajuda pra implementar o InfoProvas para o seu curso/faculdade? Pode chamar também!

## Documentação
https://devmobufrj.github.io/infoprovas-api/

## Setup local
A API usa PHP >= 7.2 e Lumen, e banco de dados MySQL. Siga os passos abaixo para configurar o ambiente
de desenvolvimento.


1. Instalar PHP, MariaDB e dependências: `sudo apt install mariadb-server php7.4 php7.4-common php7.4-cli php7.4-mbstring php7.4-mysql php7.4-zip php7.4-xml openssl curl`
2. Baixar o composer: `curl -sS https://getcomposer.org/installer -o composer-setup.php`
3. Instalar o composer: 'sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer'
4. Clonar o projeto para o seu computador (caso ainda não tenha feito).
5. Configurar usuário, senha e banco de dados do MySQL:
   `CREATE USER 'infoprovas'@'localhost' IDENTIFIED BY '';
    CREATE DATABASE infoprovas;
    GRANT ALL PRIVILEGES ON infoprovas.* TO 'infoprovas'@'localhost';
    flush privileges;`
6. Configurar o arquivo `.env` com acesso do banco de dados.
7. Na pasta do projeto, executar: `composer install`


Executar localmente: `php -S localhost:8000 -t public`

Acessar em: `http://localhost:8000`

Para usar publicamente o projeto em um servidor, é necessário configurar o projeto no apache ou nginx.
