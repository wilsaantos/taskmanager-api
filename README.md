# 📋 API de Gerenciamento de Tarefas - NestJS Challenge

## 🚀 Sobre o Projeto

Este projeto é uma API de gerenciamento de tarefas (Tasks Management API), desenvolvida como parte de um desafio técnico para avaliação de conhecimentos em **NestJS**, **Banco de Dados**, **Docker**, **Testes Unitários**, **Documentação** e **Boas práticas de DevOps**.

A API permite criar, listar, buscar, atualizar e deletar tarefas, com controle de status.

---

## 🧰 Tecnologias e Ferramentas

- [NestJS](https://nestjs.com/)
- [TypeScript](https://www.typescriptlang.org/)
- [TypeORM](https://typeorm.io/) ou [Prisma](https://www.prisma.io/)
- [PostgreSQL](https://www.postgresql.org/) ou [MySQL](https://www.mysql.com/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Swagger](https://swagger.io/)
- [Jest](https://jestjs.io/)

---

## 📦 Como rodar o projeto

### Pré-requisitos

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Git](https://git-scm.com/)

### Rodando com Docker Compose

```bash
# 1. Clone o repositório:
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

# 2. Suba a aplicação:
docker-compose up --build

# 3. Acesse a API:
# API Rodando em: http://localhost:3000
# Documentação Swagger: http://localhost:3000/api
```

---

## 🔥 Funcionalidades

- [x] Criar uma nova tarefa
- [x] Listar todas as tarefas
- [x] Buscar uma tarefa por ID
- [x] Atualizar uma tarefa
- [x] Deletar uma tarefa

Cada tarefa possui:

- **Título**
- **Descrição**
- **Status** (`PENDENTE`, `EM ANDAMENTO`, `CONCLUÍDA`)

---

## 🧪 Testes

- Testes unitários para Services.
- Testes de integração para Controllers.

### Rodar testes:

```bash
npm run test
```

---

## 🛠 Estrutura do Projeto (sugerida)

```plaintext
src/
  ├── tasks/
  │    ├── tasks.controller.ts
  │    ├── tasks.service.ts
  │    ├── tasks.module.ts
  │    ├── dto/
  │    │    ├── create-task.dto.ts
  │    │    └── update-task.dto.ts
  │    ├── entities/
  │    │    └── task.entity.ts
  │    └── enums/
  │         └── task-status.enum.ts
  ├── app.module.ts
main.ts
```

---

## 📚 Documentação Swagger

Após rodar o projeto, acesse:

```text
http://localhost:3000/api
```

A documentação inclui:

- Endpoints
- Parâmetros de entrada
- Schemas de resposta
- Exemplos de requisição

---

## 🐳 Docker

O projeto inclui:

- `Dockerfile` para a API
- `docker-compose.yml` para API + Banco de Dados

Principais variáveis de ambiente usadas:

- `DB_HOST`
- `DB_PORT`
- `DB_USER`
- `DB_PASSWORD`
- `DB_NAME`

---

## 📜 Logs

O projeto utiliza o sistema de `Logger` nativo do NestJS para:

- Registro de criação, atualização e deleção de tarefas
- Log de erros no sistema

---

## ✨ Diferenciais implementados (caso aplicável)

- [ ] Autenticação JWT
- [ ] Deploy Cloud
- [ ] Pipeline CI/CD com GitHub Actions

---

## 📄 Licença

Este projeto está sob licença privada, desenvolvido para fins de avaliação técnica.

---

**Desenvolvido com 💻 usando NestJS.**
