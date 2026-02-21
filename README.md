# Todo List API

A simple Todo List REST API using Node.js and Express with full CRUD operations. Data is stored in memory, no database required.

## API Documentation

Postman documentation is available here:
https://documenter.getpostman.com/view/51751420/2sBXcEk1FV

## Tech Stack

- **Runtime:** Node.js
- **Framework:** Express
- **Other:** uuid, dotenv

## Endpoints

- GET /api/todos - List all todos
- GET /api/todos/:id - Get a single todo
- POST /api/todos - Create a new todo
- PUT /api/todos/:id - Update a todo
- DELETE /api/todos/:id - Delete a todo

## Details

- Data is stored in memory using an array and will reset when the server restarts.
- Each todo is assigned a unique UUID on creation.
- Input validation and error handling

## Project Structure

```
backend/
├── src/
│   ├── controllers/
│   │   └── todoController.js   # CRUD logic
│   ├── data/
│   │   └── store.js            # In-memory storage
│   ├── routes/
│   │   └── todoRoutes.js       # Routes
│   └── server.js               # Express app setup
├── .env.example
├── index.js                    # Entry point
└── package.json
```


