<h1 align="center">
  Banco de dados e upload de arquivos no Node.js
</h1>

<h3 align="center">
  O projeto desenvolvido foi a criação de uma aplicação para armazenar transações financeiras de entrada e saída e permitir o cadastro e a listagem dessas transações, além de permitir a criação de novos registros no banco de dados a partir do envio de um arquivo csv.
</h3>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/thiagokrathos/database-upload">

  <img alt="GitHub stars" src="https://img.shields.io/github/stars/thiagokrathos/database-upload?style=social">
</p>

<p align="center">
  <a href="#funcionalidades">Funcionalidades</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#heavy_check_mark-configurações-necessárias">Configurações necessárias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#arrow_down_small-clonando-o-repositório">Clonando o repositório</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#beginner-iniciando-a-aplicação">Iniciando a aplicação</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#wrench-tecnologias--ferramentas--recursos">Tecnologias | Ferramentas | Recursos</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
</p>

Durante as aulas do [RocketSeat GoStack Bootcamp](https://rocketseat.com.br/bootcamp) foram aprendidos conteúdos relacionados a NodeJS junto com TypeScript, utilizando o conceito de models, repositories, services, banco de dados com o TypeORM e envio de arquivos com o Multer. Para treinar o que foi aprendido até o momento foi criada uma aplicação para gestão de transações financeiras.

### Funcionalidades

- Criação de transações financeiras de entrada e saída;
- Listagem das transações registradas;
- Criação de novos registros no banco de dados a partir do envio de um arquivo csv.

### :heavy_check_mark: Configurações necessárias

Seguem as configurações neessárias para visualizar a aplicação em sua máquina.

-  [Git](https://git-scm.com);
-  [Node](https://nodejs.org/);
-  [Yarn](https://yarnpkg.com/);
-  [Docker](https://www.docker.com/docker-community).

### :arrow_down_small: Clonando o repositório
1. Pelo terminal, acesse o diretório em que deseja ter o repositório clonado e execute o comando a seguir.
```bash
# clonando o repositório
git clone https://github.com/thiagokrathos/banco-de-dados-e-upload-nodejs
```
### :beginner: Iniciando a aplicação
1. Crie e inicie o serviço de bancos de dados `postgres` utilizando os comandos a seguir. O nome e a senha são uma sugestão e podem ser alterados conforme sua preferência.
```bash
# criando serviço de banco de dados postgres
docker run --name gostack_postgres -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres

# iniciando o serviço de banco de dados
docker start gostack_postgres
```
2. Pelo terminal, acesse o diretório do repositório clonado e execute os comandos abaixo.
```bash
# instalando as dependências
yarn install

# executando as migrations
yarn typeorm migration:run

# iniciando o servidor
yarn dev:server
```
### :mag: Realizando os testes
1. Foi usado um template que contém testes para orientar o que esperava-se dos blocos de códigos a serem programados. Para verificar se qualquer alteração realizada atende aos requisitos solicitados, acesse o terminal e executo o seguinte comando:
```bash
# testando atendimento aos requisitos
yarn test
```
Você pode utilizar ferramentas como o Insomnia, o Postman e o Postwoman para testar as rotas e requisições configuradas e o DBeaver para acompanhar a criação das tabelas e registros no banco de dados.

### :wrench: Tecnologias | Ferramentas | Recursos

Esse projeto foi desenvolvido utilizando os seguintes recursos:

-  [CSV Parser](https://csv.js.org/parse/);
-  [Dotenv](https://www.npmjs.com/package/dotenv);
-  [Editor Config](https://editorconfig.org/);
-  [Eslint](https://eslint.org/);
-  [Express](https://expressjs.com/);
-  [Jest](https://jestjs.io/);
-  [Multer](https://github.com/expressjs/multer);
-  [Pg](https://www.npmjs.com/package/pg);
-  [Node.js](https://nodejs.org/en/);
-  [Prettier](https://prettier.io/)
-  [Supertest](https://github.com/visionmedia/supertest);
-  [TypeORM](https://typeorm.io/#/);
-  [TypeScript](https://www.typescriptlang.org/);


---

Feito por Thiago Almeida :blue_heart: Contato: https://www.linkedin.com/in/thiago-almeida-54140b128 :blush:
