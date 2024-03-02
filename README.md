# Simple Todo API README

This repository contains the source code for a simple Todo API built with Next.js. The API interacts with a mock data source at `https://jsonplaceholder.typicode.com/todos` to perform CRUD operations on todo items. It demonstrates the use of `GET`, `POST`, `PUT`, and `DELETE` methods to manage todo items.

## Features

- Fetch all todo items or a specific todo by ID.
- Add a new todo item.
- Update an existing todo item.
- Delete a todo item.

## Setup

1. Clone the repository to your local machine.
2. Install the necessary dependencies by running `npm install` or `yarn` in the project directory.
3. Create a `.env` file in the root of the project and add your API key as `DATA_API_KEY=your_api_key_here`.

## Usage

### Fetch Todos

- **GET** `/api/todos`: Fetches all todos.
- **GET** `/api/todos/{id}`: Fetches a todo item by ID.

### Manage Todos

- **POST** `/api/todos`: Adds a new todo item. Requires `userId` and `title` in the request body.
- **PUT** `/api/todos/{id}`: Updates an existing todo item. Requires `userId`, `id`, `title`, and `completed` in the request body.
- **DELETE** `/api/todos/{id}`: Deletes a todo item by ID.

## Environment Variables

- `DATA_API_KEY`: API key for authentication with the data source.
