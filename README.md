**Spring Boot Simple API Exercise**

**Description:**
<br>
This project implements a RESTful API using Spring Boot to manage a collection of books. <br>
The API supports CRUD operations: Create, Read, Update, and Delete.

**Project Setup** <br>
Port: Running on http://localhost:8080/books  <br>
PostgreSQL Database: JDBC URL: jdbc:postgresql://localhost:5432/BookApi <br>
User Name: postgres <br>
Password: Global <br>

**API Endpoints**

POST - Adding Book URL: http://localhost:8080/books <br>
Data: <br>

json <br>
{ 
"title": "To Kill a Mockingbird", <br>
"author": "Harper Lee", <br>
"isbn": "9780060935467" <br>
}

**GET - Get All Books**  <br>
URL: http://localhost:8080/books

**GET - Get Book By ID** <br>
URL: http://localhost:8080/books/:bookId <br>
Example: http://localhost:8080/books/1

**PUT - Update Book By ID** <br>
URL: http://localhost:8080/books/:bookId <br>
Example: http://localhost:8080/books/1 Data:

**DELETE - Delete Book By ID** <br>
URL: http://localhost:8080/books/:bookId  <br>
Example: http://localhost:8080/books/1

**Testing Run the application** <br>
Open Postman Hit the above-mentioned endpoints and check the responses. <br>
Error Handling If Book ID is not found: Response: 404 Not Found Message: "Book not found with id : {bookId}" Status Code: 404  <br>
If Book ID is found: Response: 200 OK with the book details.

