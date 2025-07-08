# 🏥 Backend CRUD - Farmácia

Este é um projeto de **backend** realizado durante o bootcamp da Generation, focado na criação de um sistema **CRUD (Create, Read, Update, Delete)** para **produtos e categorias de uma farmácia**, desenvolvido com **NestJS** e **TypeScript**. A aplicação possui uma estrutura modular, seguindo boas práticas de desenvolvimento, e utiliza **MySQL** como banco de dados. A API pode ser testada com o **Insomnia**.

---

## 🚀 Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)
- [NestJS](https://nestjs.com/)
- [TypeScript](https://www.typescriptlang.org/)
- [MySQL](https://www.mysql.com/)
- [Insomnia](https://insomnia.rest/) – para testes da API
- [NPM](https://www.npmjs.com/) – gerenciador de pacotes

---

## 📁 Estrutura do Projeto

```
src/
├── categoria/
│   ├── categoria.controller.ts
│   ├── categoria.entity.ts
│   ├── categoria.module.ts
│   ├── categoria.service.ts
├── produto/
│   ├── produto.controller.ts
│   ├── produto.entity.ts
│   ├── produto.module.ts
│   ├── produto.service.ts
├── app.module.ts
```

## 🛠️ Funcionalidades

### ✅ CRUD de Produtos

- `GET /produtos`: Lista todos os produtos
- `GET /produtos/:id`: Retorna um produto por ID
- `POST /produtos`: Cadastra um novo produto
- `PUT /produtos/:id`: Atualiza um produto existente
- `DELETE /produtos/:id`: Deleta um produto
- `GET /produtos/nome/:nome`: Busca produtos por nome
- `POST /produtos/:id/desconto`: Aplica 50% de desconto no preço de um produto

### ✅ CRUD de Categorias

- `GET /categorias`: Lista todas as categorias
- `GET /categorias/:id`: Retorna uma categoria por ID
- `POST /categorias`: Cadastra uma nova categoria
- `PUT /categorias/:id`: Atualiza uma categoria existente
- `DELETE /categorias/:id`: Deleta uma categoria
- `GET /categorias/nome/:nome`: Busca categorias por nome

## 🔗 Relacionamento

O projeto implementa o relacionamento:

- **Categoria (1)** → **(N) Produtos**  
Cada produto pertence a uma única categoria, enquanto uma categoria pode ter vários produtos.

---

## ✅ Testes

A API pode ser testada utilizando o **Insomnia** ou qualquer outra ferramenta de testes REST.

