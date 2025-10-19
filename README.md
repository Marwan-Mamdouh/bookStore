# BookStore Backend API

This is a backend API for a bookstore application built with JavaScript, Express.js, and MongoDB. The API provides endpoints to manage books and authors, including CRUD (Create, Read, Update, Delete) operations. It uses MongoDB as the database and includes middleware for handling requests and responses.

## Table of Contents
- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [API Endpoints](#api-endpoints)
- [Environment Variables](#environment-variables)
- [Contributing](#contributing)

## Features
- Create, read, update, and delete books and authors.
- RESTful API design with clear and consistent endpoints.
- MongoDB integration for persistent data storage.
- Middleware for request validation and error handling.
- Environment variable configuration for secure and flexible setup.

## Technologies
- **Node.js**: JavaScript runtime for server-side development.
- **Express.js**: Web framework for building the API.
- **MongoDB**: NoSQL database for storing books and authors.
- **Mongoose**: ODM library for MongoDB.
- **dotenv**: For managing environment variables.

## Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Marwan-Mamdouh/bookStore.git
   cd bookStore
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Set up environment variables**:
   Create a `.env` file in the root directory and add the following:
   ```
   PORT=3000
   MONGODB_URI=mongodb://localhost:27017/bookstore
   ```
   Replace `MONGODB_URI` with your MongoDB connection string.

4. **Run MongoDB**:
   Ensure MongoDB is installed and running locally or provide a cloud-based MongoDB URI (e.g., MongoDB Atlas).

5. **Start the server**:
   ```bash
   npm start
   ```
   The API will be available at `http://localhost:3000`.

## API Endpoints
### Books
- **GET /api/books**: Retrieve all books.
- **GET /api/books/:id**: Retrieve a book by ID.
- **POST /api/books**: Create a new book.
- **PUT /api/books/:id**: Update a book by ID.
- **DELETE /api/books/:id**: Delete a book by ID.

### Authors
- **GET /api/authors**: Retrieve all authors.
- **GET /api/authors/:id**: Retrieve an author by ID.
- **POST /api/authors**: Create a new author.
- **PUT /api/authors/:id**: Update an author by ID.
- **DELETE /api/authors/:id**: Delete an author by ID.

## Environment Variables
The `.env` file should include:
- `PORT`: The port on which the server runs (default: 3000).
- `MONGODB_URI`: The MongoDB connection string.

Example `.env`:
```
PORT=3000
MONGODB_URI=mongodb://localhost:27017/bookstore
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.
