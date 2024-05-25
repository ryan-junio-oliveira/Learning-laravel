# Manual de Comandos Artisan do Laravel

Este é um guia abrangente para os principais comandos do Artisan do Laravel e uma visal geral de sua respectiva estrutura de pastas.

## Comandos Gerais

- `php artisan list`: Mostra a lista de todos os comandos Artisan.
- `php artisan help <comando>`: Mostra a ajuda para um comando Artisan.
- `php artisan migrate`: Executa as migrações de banco de dados.
- `php artisan migrate:fresh`: Executa as migrações de banco de dados e remove todas as tabelas existentes.
- `php artisan make:migration`: Cria um novo arquivo de migração.
- `php artisan make:model`: Cria um novo modelo Eloquent.
- `php artisan make:controller`: Cria um novo controlador.
- `php artisan make:repository`: Cria um novo repositório.
- `php artisan tinker`: Abre o Tinker, um REPL para o Laravel.
- `php artisan queue:work`: Executa as tarefas em segundo plano.
- `php artisan schedule:run`: Executa o agendamento de tarefas.

## Chamando os Comandos de Fora do CLI

- `Artisan::call('comando', ['--opção' => 'valor'])`: Executa um comando Artisan de fora do CLI.
- `Artisan::queue('comando', ['--opção' => 'valor'])`: Enfileira um comando Artisan para que seja processado em segundo plano pelo seu queue workers.

## Agendando Comandos Artisan

- `* * * * * php /path/to/artisan schedule:run 1>> /dev/null 2>&1`: Define um agendamento para executar o comando `schedule:run` todo minuto.

# Panorama Geral dos Arquivos do Projeto Laravel

O Laravel é um framework PHP que fornece uma estrutura robusta para desenvolver aplicações web. Quando você cria um novo projeto Laravel, ele gera uma estrutura de pastas e arquivos que ajudam a organizar o seu código. Aqui está um panorama geral sobre os arquivos e pastas do projeto Laravel:

### Pastas

- **app**: Esta pasta contém o código do aplicativo, incluindo os controladores, modelos, repositórios e serviços.
- **bootstrap**: Esta pasta contém arquivos de inicialização do aplicativo, incluindo o arquivo `app.php` que define as configurações do aplicativo.
- **config**: Esta pasta contém arquivos de configuração do aplicativo, incluindo as configurações de database, autenticação e outras configurações.
- **database**: Esta pasta contém arquivos de schema do banco de dados, incluindo as tabelas e relacionamentos.
- **public**: Esta pasta contém os arquivos públicos do aplicativo, incluindo a página de entrada e os arquivos de estilo e script.
- **resources**: Esta pasta contém arquivos de recursos do aplicativo, incluindo as views, linguagens e imagens.
- **routes**: Esta pasta contém arquivos de rotas do aplicativo, incluindo as rotas de entrada e as rotas de saída.
- **storage**: Esta pasta contém arquivos de armazenamento do aplicativo, incluindo as imagens e arquivos de upload.
- **tests**: Esta pasta contém arquivos de testes do aplicativo, incluindo os testes unitários e de integração.
- **vendor**: Esta pasta contém os pacotes de terceiros instalados no aplicativo, incluindo os pacotes de bibliotecas e frameworks.

### Arquivos

- **app/Http/Controllers**: Esta pasta contém os controladores do aplicativo, incluindo os controladores de entrada e os controladores de saída.
- **app/Http/Requests**: Esta pasta contém os pedidos do aplicativo, incluindo os pedidos de entrada e os pedidos de saída.
- **app/Models**: Esta pasta contém os modelos do aplicativo, incluindo os modelos de dados e os modelos de negócios.
- **app/Repositories**: Esta pasta contém os repositórios do aplicativo, incluindo os repositórios de dados e os repositórios de negócios.
- **app/Services**: Esta pasta contém os serviços do aplicativo, incluindo os serviços de autenticação e os serviços de armazenamento.
- **bootstrap/app.php**: Este arquivo define as configurações do aplicativo, incluindo as configurações de database e as configurações de autenticação.
- **config/app.php**: Este arquivo define as configurações do aplicativo, incluindo as configurações de database e as configurações de autenticação.
- **database/migrations**: Esta pasta contém arquivos de migração do banco de dados, incluindo as migrações de schema e as migrações de dados.
- **public/index.php**: Este arquivo é a página de entrada do aplicativo, incluindo a lógica de inicialização do aplicativo.
- **resources/views**: Esta pasta contém as views do aplicativo, incluindo as views de entrada e as views de saída.
- **routes/web.php**: Este arquivo define as rotas do aplicativo, incluindo as rotas de entrada e as rotas de saída.
- **storage/app/public**: Esta pasta contém os arquivos públicos do aplicativo, incluindo as imagens e arquivos de upload.
- **tests/Feature**: Esta pasta contém os testes de feature do aplicativo, incluindo os testes de integração e os testes de usuário.
- **tests/Unit**: Esta pasta contém os testes unitários do aplicativo, incluindo os testes de unidade e os testes de integração.

Esses comandos abrangem uma variedade de funcionalidades do Artisan do Laravel para ajudar no gerenciamento eficiente de imagens, containers, redes e volumes Docker. Explore mais opções e detalhes na documentação oficial do Laravel para aprofundar seu conhecimento e aproveitar ao máximo essa poderosa ferramenta de virtualização de contêineres.

Acessar o container
```sh
docker-compose exec app bash
```
