# JavaSpring CRUD
Projeto usando java&spring, uma forma fácil de connstruir uma api-rest para que o front possa consumir.

## Instalação

1. Clonar o repositório:

```bash
$ git clone git@github.com:fernandopdeandrade/crud-java-spring.git
```

2. Instalar as dependências com Maven

## Use

1. Iniciar o applicaivo com Maven
2. API acessível em: http://localhost:8080


## Endpoints da API
Endpoints usados no projeto:

```markdown
GET /product - Buscar todos os produtos do banco.

POST /product - Registrar um novo produto.

PUT /product - Alterar ou editar um produto do banco, é necessário passar o id do produto no body.

DELETE /product/inative/{id} - Inativar um produto sem excluir do banco de dados.

DELETE /product/delete/{id} - Excluir um produto permanentemente do banco de dados.
```

## Banco de dados
O projeto usa PostgresSQL como banco de dados. As migrações de banco de dados necessárias são gerenciadas usando Flyway.

Intale o PostgreSQL, caso queira usar instalado na máquina: [click here](https://www.postgresql.org/download/).

## Certifique-se de ter o Docker instalado na máquina caso opte.

- Você pode usar o docker para criar um banco de dados, assim usará apenas o container do postgreSQL.
- Você pode usar o Dbeaver para gerenciar o seu banco de dados também, caso queira: [click here](https://dbeaver.io/download/)


```bash
$ docker-compose up
```
Depois de executado e rodando, acesse: http://localhost:15432

Digite o e-mail e a senha configurados em: [Arquivo](./docker-compose.yml).

Para instalar o Docker localmente: [click here](https://www.docker.com/products/docker-desktop/).
