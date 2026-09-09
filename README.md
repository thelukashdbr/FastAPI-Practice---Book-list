# 📚 FastAPI Books API

A simple REST API project built with **FastAPI**, following the lessons and implementation presented in the Udemy course **[FastAPI - The Complete Course](https://www.udemy.com/course/fastapi-the-complete-course/)**.

> 🇺🇸 English | 🇧🇷 [Português](README-pt-BR.md)

## 📖 About the Project

This project was created as a hands-on practice exercise while following the FastAPI course.

The application consists of a simple **book list API**, designed to practice the fundamentals of building REST APIs with FastAPI.

The project covers:

* FastAPI project setup;
* REST API endpoints;
* CRUD operations;
* Data validation with Pydantic;
* HTTP exception handling;
* HTTP status codes;
* Automatic API documentation.

## 🚀 Features

The API provides basic CRUD operations for books.

### Create a book

```http
POST /books
```

Creates a new book.

### Get all books

```http
GET /books
```

Returns the list of available books.

### Get a book

```http
GET /books/{book_id}
```

Returns a specific book by its ID.

### Update a book

```http
PUT /books/{book_id}
```

Updates an existing book.

### Delete a book

```http
DELETE /books/{book_id}
```

Removes a book from the list.

## ✅ Data Validation

The project uses **Pydantic** models to validate incoming request data.

This helps ensure that the API receives data in the expected format and provides automatic validation errors when invalid data is submitted.

## ⚠️ HTTP Exception Handling

The API also demonstrates how to handle HTTP exceptions using FastAPI.

For example, when requesting a book that does not exist, the API returns an appropriate HTTP error response such as:

```json
{
  "detail": "Book not found"
}
```

## 📊 HTTP Status Codes

The project demonstrates the use of different HTTP status codes according to the result of each operation.

| Status Code                | Description                                          |
| -------------------------- | ---------------------------------------------------- |
| `200 OK`                   | Request completed successfully                       |
| `201 Created`              | Resource created successfully                        |
| `204 No Content`           | Request completed successfully with no response body |
| `404 Not Found`            | Requested resource was not found                     |
| `422 Unprocessable Entity` | Request data failed validation                       |

## 🛠️ Technologies

* Python
* FastAPI
* Pydantic
* Uvicorn

## 📁 Project Structure

```text
.
├── main.py
├── requirements.txt
├── README.md
└── README-pt-BR.md
```

## ▶️ Running the Project

### 1. Clone the repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd <PROJECT_FOLDER>
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

On Windows:

```bash
venv\Scripts\activate
```

On Linux/macOS:

```bash
source venv/bin/activate
```

### 3. Install the dependencies

```bash
pip install -r requirements.txt
```

### 4. Start the application

```bash
uvicorn main:app --reload
```

The API will be available at:

```text
http://127.0.0.1:8000
```

## 📑 API Documentation

FastAPI automatically generates interactive API documentation.

### Swagger UI

```text
http://127.0.0.1:8000/docs
```

### ReDoc

```text
http://127.0.0.1:8000/redoc
```

## 🎯 Learning Goals

The main goal of this project was to practice the fundamentals of API development with FastAPI:

**Project Setup → Endpoints → CRUD → Validation → Exceptions → Status Codes**

This project represents a learning exercise rather than an original application. The implementation was reproduced while following the course material in order to reinforce the concepts presented throughout the lessons.

## 🎓 Course Reference

This project was developed by following the course:

**FastAPI - The Complete Course**
Udemy: https://www.udemy.com/course/fastapi-the-complete-course/

The original implementation and teaching materials belong to the course instructor and Udemy course.

## 👨‍💻 About This Repository

This repository is part of my learning journey with **Python and FastAPI** and was created for educational purposes.
