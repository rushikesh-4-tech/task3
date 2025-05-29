# Simple Book API with Node.js and Express

This project is a basic RESTful API built using Node.js and Express.js. It allows you to manage a collection of books with full CRUD operations — Create, Read, Update, and Delete — all stored in memory.

## Features

* Get a list of all books
* Add a new book
* Update an existing book by ID
* Delete a book by ID

## Technologies Used

* Node.js
* Express.js

## Project Structure

book-api/
├── index.js        # Main server file (contains all API routes)
├── package.json    # Project metadata and dependencies
└── README.md       # Project documentation

## How to Run the Project

### 1. Initialize a Node.js project

```
npm init -y
```

### 2. Install Express.js

```
npm install express
```

### 3. Create your main file

Create a file called `index.js` and paste the server code there.

### 4. Start the Server

```
node index.js
```

Server will run on:

```
http://localhost:3000
```

## API Endpoints

| Method | Endpoint     | Description         |
| ------ | ------------ | ------------------- |
| GET    | `/books`     | Get all books       |
| POST   | `/books`     | Add a new book      |
| PUT    | `/books/:id` | Update a book by ID |
| DELETE | `/books/:id` | Delete a book by ID |
| GET    | `/`          | Welcome message     |

## Example JSON for POST/PUT

```
{
  "title": "The Hobbit",
  "author": "J.R.R. Tolkien"
}
```

## Steps to Create This API

1. Set up Node.js project with `npm init -y`.
2. Installed Express using `npm install express`.
3. Created an Express server using `express()` and added middleware to parse JSON.
4. Set up an in-memory array to store books and auto-increment book IDs.
5. Created RESTful routes:

   * GET /books
   * POST /books
   * PUT /books/\:id
   * DELETE /books/\:id
6. Handled edge cases like missing data or invalid book IDs.
7. Tested the API using Postman.

## Notes

* This project does not use a database; books are stored in memory and reset when the server restarts.
* For production, you would typically connect this to a database like MongoDB or PostgreSQL.

## Feedback

Feel free to improve or extend this project — add validation, connect a database, or create a frontend!
![Uploading Screenshot 2025-05-29 212802.png…]()
