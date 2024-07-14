**Spring Boot Simple API Exercise**

**Description**
This project implements a RESTful API using Spring Boot to manage a collection of books. The API supports CRUD operations: Create, Read, Update, and Delete.

**Project Setup**
Port: Running on http://localhost:8080/books
PostgreSQL Database: JDBC URL: jdbc:postgresql://localhost:5432/BookApi 
User Name: postgres 
Password: Global

**API Endpoints**

POST - Adding Book URL: http://localhost:8080/books Data:

json 
{ 
"title": "To Kill a Mockingbird",
"author": "Harper Lee",
"isbn": "9780060935467"
}

**GET - Get All Books**
URL: http://localhost:8080/books

**GET - Get Book By ID**
URL: http://localhost:8080/books/:bookId Example: http://localhost:8080/books/1

**PUT - Update Book By ID**
URL: http://localhost:8080/books/:bookId Example: http://localhost:8080/books/1 Data:

**DELETE - Delete Book By ID**
URL: http://localhost:8080/books/:bookId Example: http://localhost:8080/books/1

**Testing Run the application**
Open Postman Hit the above-mentioned endpoints and check the responses.
Error Handling If Book ID is not found: Response: 404 Not Found Message: "Book not found with id : {bookId}" Status Code: 404 
If Book ID is found: Response: 200 OK with the book details.

