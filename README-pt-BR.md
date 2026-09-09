# 📚 FastAPI Books API

Um projeto simples de API REST desenvolvido com **FastAPI**, seguindo as aulas e a implementação apresentada no curso da Udemy **[FastAPI - The Complete Course](https://www.udemy.com/course/fastapi-the-complete-course/)**.

> 🇺🇸 [English](README.md)

## 📖 Sobre o Projeto

Este projeto foi desenvolvido como um exercício prático de aprendizado durante o acompanhamento do curso de FastAPI.

A aplicação consiste em uma API simples para gerenciamento de uma **lista de livros**, criada para praticar os fundamentos do desenvolvimento de APIs REST com FastAPI.

O projeto aborda:

* Configuração inicial de um projeto FastAPI;
* Criação de endpoints REST;
* Operações CRUD;
* Validação de dados com Pydantic;
* Tratamento de exceções HTTP;
* Utilização de HTTP status codes;
* Documentação automática da API.

## 🚀 Funcionalidades

A API disponibiliza operações básicas de CRUD para livros.

### Criar um livro

```http
POST /books
```

Cria um novo livro.

### Listar livros

```http
GET /books
```

Retorna a lista de livros disponíveis.

### Buscar um livro

```http
GET /books/{book_id}
```

Retorna um livro específico através do seu ID.

### Atualizar um livro

```http
PUT /books/{book_id}
```

Atualiza um livro existente.

### Excluir um livro

```http
DELETE /books/{book_id}
```

Remove um livro da lista.

## ✅ Validação de Dados

O projeto utiliza modelos do **Pydantic** para realizar a validação dos dados recebidos nas requisições.

Isso garante que os dados estejam no formato esperado pela API e permite que erros de validação sejam retornados automaticamente quando informações inválidas são enviadas.

## ⚠️ Tratamento de Exceções HTTP

A API também demonstra como realizar o tratamento de exceções HTTP utilizando o FastAPI.

Por exemplo, ao solicitar um livro que não existe, a API retorna uma resposta de erro HTTP apropriada, como:

```json
{
  "detail": "Book not found"
}
```

## 📊 HTTP Status Codes

O projeto demonstra a utilização de diferentes status codes de acordo com o resultado de cada operação.

| Status Code                | Descrição                                            |
| -------------------------- | ---------------------------------------------------- |
| `200 OK`                   | Requisição concluída com sucesso                     |
| `201 Created`              | Recurso criado com sucesso                           |
| `204 No Content`           | Operação concluída sem conteúdo no corpo da resposta |
| `404 Not Found`            | Recurso solicitado não encontrado                    |
| `422 Unprocessable Entity` | Dados enviados não passaram pela validação           |

## 🛠️ Tecnologias

* Python
* FastAPI
* Pydantic
* Uvicorn

## 📁 Estrutura do Projeto

```text
.
├── main.py
├── requirements.txt
├── README.md
└── README-pt-BR.md
```

## ▶️ Como Executar o Projeto

### 1. Clone o repositório

```bash
git clone <URL_DO_SEU_REPOSITORIO>
cd <PASTA_DO_PROJETO>
```

### 2. Crie um ambiente virtual

```bash
python -m venv venv
```

No Windows:

```bash
venv\Scripts\activate
```

No Linux/macOS:

```bash
source venv/bin/activate
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

### 4. Execute a aplicação

```bash
uvicorn main:app --reload
```

A API estará disponível em:

```text
http://127.0.0.1:8000
```

## 📑 Documentação da API

O FastAPI gera automaticamente uma documentação interativa da API.

### Swagger UI

```text
http://127.0.0.1:8000/docs
```

### ReDoc

```text
http://127.0.0.1:8000/redoc
```

## 🎯 Objetivos de Aprendizado

O principal objetivo deste projeto foi praticar os fundamentos do desenvolvimento de APIs com FastAPI:

**Setup do Projeto → Endpoints → CRUD → Validação → Exceptions → Status Codes**

Este projeto representa um exercício de aprendizado e não uma aplicação original. A implementação foi reproduzida acompanhando o conteúdo do curso com o objetivo de reforçar os conceitos apresentados durante as aulas.

## 🎓 Referência do Curso

Este projeto foi desenvolvido seguindo o curso:

**FastAPI - The Complete Course**
Udemy: https://www.udemy.com/course/fastapi-the-complete-course/

<img width="1600" height="1190" alt="image" src="https://github.com/user-attachments/assets/bf8faed8-557c-41df-bddf-4da5b9330515" />


## 👨‍💻 Sobre este Repositório

Este repositório faz parte da minha jornada de aprendizado em **Python e FastAPI** e foi criado para fins educacionais.
