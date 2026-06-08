# SGTA - Sistema de Gerenciamento de Tarefas Acadêmicas

## Sobre o Projeto

O SGTA (Sistema de Gerenciamento de Tarefas Acadêmicas) é uma API desenvolvida em Python utilizando Django e Django REST Framework para gerenciamento de tarefas acadêmicas.

O sistema permite o cadastro, consulta, atualização e exclusão de usuários e tarefas, utilizando PostgreSQL como banco de dados e Docker para containerização da aplicação.

---

## Tecnologias Utilizadas

* Python 3
* Django
* Django REST Framework
* PostgreSQL
* Docker
* Docker Compose
* Git
* GitHub

---

## Funcionalidades

### Usuários

* Cadastrar usuário
* Consultar usuário
* Atualizar usuário
* Excluir usuário

### Tarefas

* Cadastrar tarefa
* Consultar tarefa
* Atualizar tarefa
* Excluir tarefa
* Associar tarefas a usuários

---

## Estrutura do Projeto

```text
SGTA/
│
├── config/
├── tarefas/
├── usuarios/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── entrypoint.sh
└── manage.py
```

---

## Banco de Dados

O projeto utiliza PostgreSQL executando em container Docker.

Principais vantagens:

* Persistência dos dados
* Ambiente padronizado
* Facilidade de implantação
* Integração com Django ORM

---

## Executando o Projeto com Docker

### Clonar o Repositório

```bash
git clone https://github.com/Arthur21-star/API-PYTHON-PostgreSQL.git
```

### Entrar na Pasta do Projeto

```bash
cd API-PYTHON-PostgreSQL
```

### Construir e Executar os Containers

```bash
docker compose up --build
```

---

## Acesso à Aplicação

Painel Administrativo:

```text
http://localhost:8000/admin/
```

API:

```text
http://localhost:8000/
```

---

## Docker Hub

Imagem publicada:

```bash
docker pull arthurzinho/sgta-web
```

Link:

https://hub.docker.com/repository/docker/arthurzinho/sgta-web

---

## Testes

Executar os testes da aplicação:

```bash
docker compose exec web python manage.py test
```

---

## Autor

Arthur Soares

Projeto desenvolvido para a disciplina de Programação Backend.

