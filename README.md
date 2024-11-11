# Sistema de Gerenciamento de Tarefas

Um sistema de gerenciamento de tarefas desenvolvido com Laravel, que inclui funcionalidades de cadastro de usuários com confirmação de e-mail e notificação ao criar novas tarefas. O sistema foi criado utilizando o Laravel UI.

## Funcionalidades

- **Cadastro de Usuários**: Os usuários podem se cadastrar e recebem um link de confirmação por e-mail para verificar sua conta.
- **Gerenciamento de Tarefas**: Os usuários podem criar, editar e excluir tarefas.
- **Notificação por E-mail**: Envio de e-mails de notificação ao cadastrar novas tarefas.

## Tecnologias Utilizadas

- [Laravel](https://laravel.com/) - Framework PHP
- [Laravel UI](https://github.com/laravel/ui) - Scaffold de autenticação e UI
- [Laravel Mail](https://laravel.com/docs/8.x/mail) - Envio de e-mails

## Pré-requisitos

- PHP >= 7.3
- Composer
- MySQL

## Instalação

1. Clone o repositório:
   ```sh
   https://github.com/victtorferreira/Gereciador-de-Tarefas.git
2. Instale as dependências:
    ```sh
    composer install
3. Configure o arquivo .env com as informações do seu banco de dados e servidor de e-mail:
    ```sh
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=seu_banco_de_dados
    DB_USERNAME=seu_usuario
    DB_PASSWORD=sua_senha

    MAIL_MAILER=smtp
    MAIL_HOST=smtp.mailtrap.io
    MAIL_PORT=2525
    MAIL_USERNAME=seu_usuario
    MAIL_PASSWORD=sua_senha
    MAIL_ENCRYPTION=null
    MAIL_FROM_ADDRESS=seu_email@example.com
    MAIL_FROM_NAME="${APP_NAME}"
4. Execute as migrações e seeders:
    ```sh
    php artisan migrate --seed
5. Inicie o servidor de desenvolvimento:
    ```sh
    php artisan serve    