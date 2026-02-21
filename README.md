# Todo List API

A simple REST API for managing a todo list, built with Node.js and Express. Data is stored in memory, no database required.

## API Documentation

Postman documentation is available here:
https://documenter.getpostman.com/view/51751420/2sBXcEk1FV

## Tech Stack

- **Runtime:** Node.js
- **Framework:** Express
- **Other:** uuid, dotenv

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

## Notes

- Data is stored in memory and will reset when the server restarts.
- Each todo is assigned a unique UUID on creation.
- Duplicate todo titles are not allowed.
