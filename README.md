# Book Management API

This is a simple RESTful API built using Node.js and Express.js that allows you to manage a collection of books in memory.

## Features

- **GET /books** – Retrieve all books
- **POST /books** – Add a new book
- **PUT /books/:id** – Update a book by ID
- **DELETE /books/:id** – Delete a book by ID

## Requirements

- [Node.js](https://nodejs.org/) (v12 or above)

## Installation

1. Clone the repository or download the ZIP.
2. Navigate to the project folder:

   ```bash
   cd Task\ 3
   ```

3. Install dependencies:

   ```bash
   npm install express
   ```

## Usage

Start the server:

```bash
node server.js
```

By default, the server runs at `http://localhost:3000`.

## API Endpoints

### GET /books

Returns all books.

**Response:**
```json
[
  { "id": 1, "title": "Book Title", "author": "Author Name" }
]
```

### POST /books

Adds a new book.

**Request Body:**
```json
{
  "title": "New Book",
  "author": "Author Name"
}
```

### PUT /books/:id

Updates an existing book by ID.

**Request Body:**
```json
{
  "title": "Updated Title",
  "author": "Updated Author"
}
```

### DELETE /books/:id

Deletes a book by ID.

## Notes

- This project uses in-memory storage. All data will be lost when the server restarts.
- You can use tools like Postman or the [REST Client extension](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) in VS Code to test the API using the included `test.rest` file.
