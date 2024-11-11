# API de Registro de Usuários

Esta é uma **API RESTful** para gerenciamento de usuários, permitindo o **registro**, **login** e **armazenamento de dados** em **MongoDB**. Criada para ser integrada com uma aplicação frontend de outro repositório, a API facilita a autenticação e o gerenciamento de usuários de forma simples e segura.

## Funcionalidades

- **Registro de Usuários**: Criação de novos usuários com validação de dados (e-mail único, senha segura).
- **Autenticação de Usuários**: Login com **JWT (JSON Web Tokens)** para autenticação segura.
- **Armazenamento no MongoDB**: Usuários armazenados de forma segura no banco de dados **MongoDB**.
- **Validação de Dados**: Verificação de campos obrigatórios, como e-mail válido e senha forte.
- **Rotas protegidas**: Middleware de autenticação para garantir que apenas usuários autenticados acessem determinadas rotas.

## Tecnologias Utilizadas

- **Node.js**: Ambiente de execução JavaScript para o backend.
- **Express.js**: Framework para construir a API RESTful.
- **MongoDB**: Banco de dados NoSQL para armazenar informações dos usuários.
- **Mongoose**: Biblioteca ODM (Object Data Modeling) para facilitar a interação com o MongoDB.

## Endpoints

A API expõe o seguinte endpoint principais para interagir com o sistema:

- **POST** `/api/auth/register`: Criação de novos usuários (parâmetros: `nome`, `email`, `senha`).
