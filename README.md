# Front-end CRUD com Angular e integração com Spring Boot

Este repositório contém o front-end da aplicação CRUD, desenvolvido com **Angular 17**. Ele foi projetado para interagir com uma **API RESTful** construída com **Spring Boot** e **Java 17**. O repositório da **API** pode ser encontrado [aqui](https://github.com/claubermartins/back-crud).

O foco deste repositório é demonstrar a integração entre o front-end e o back-end, aproveitando as funcionalidades do Angular e a comunicação com a **API REST**.

---

## 💻 Tecnologias

- **Angular 17**
- **Angular Material**
- **RxJS**
- **TypeScript**
- **HTML/SCSS**

---

## Funcionalidades do Front-end

- ✅ **Componentes Standalone** (Angular v16+)
- ✅ **Componentes do Angular Material**
- ✅ **Lista de todos os cursos com paginação**
- ✅ **Formulário para atualizar/criar cursos com aulas** (has-many - **FormArray**)
- ✅ **Tela somente para visualização**
- ✅ **TypedForms** (Angular v14+)
- ✅ **Presentational x Smart Components**

---

## 🚀 Como executar o projeto

### Executando o Back-end

Antes de executar o front-end, você precisa garantir que o back-end esteja rodando.

Siga as instruções para executar o back-end da aplicação:

1. **Clone o repositório do back-end**:  
   ```bash
   git clone https://github.com/claubermartins/back-crud
   ```
   
2. **Siga as instruções do back-end** para subir a **API** e o banco de dados utilizando **Docker Compose**. A **API** estará disponível em **http://localhost:8080**.

---

### Executando o Front-end

1. **Clone este repositório**:
   Clone este repositório para sua máquina local:
   ```bash
   git clone https://github.com/claubermartins/front-crud
   cd front-crud
   ```

2. **Instalar dependências**:
   Instale as dependências necessárias usando o **NPM**:
   ```bash
   npm install
   ```

3. **Executar o projeto**:
   Execute o **Angular** para iniciar o servidor de desenvolvimento e configurar o proxy para o back-end:
   ```bash
   npm run start
   ```

   Isso iniciará o front-end no **http://localhost:4200**, enquanto o back-end estará rodando em **http://localhost:8080**.

---

## 🌐 Integração Front-end com Back-end

A comunicação entre o front-end e o back-end é feita através de requisições **HTTP** usando **HttpClient** do **Angular**. Algumas das funcionalidades que integram o front-end com o back-end incluem:

- **Listagem de Cursos**: O front-end faz uma requisição **GET** para a **API** para buscar todos os cursos disponíveis, com suporte a paginação.
- **Cadastro e Atualização de Cursos**: Formulários no front-end enviam dados via **POST** ou **PUT** para a **API**, que realiza a persistência dos cursos e suas aulas no banco de dados.
- **Exibição de Detalhes**: O front-end consome os dados das aulas e cursos da **API** para exibição detalhada, respeitando as relações **Has-Many** entre entidades.

A **API** do back-end fornece endpoints **RESTful** para realizar operações **CRUD** (Create, Read, Update, Delete) sobre os cursos e aulas, e a comunicação é gerenciada por **services** no **Angular**.

