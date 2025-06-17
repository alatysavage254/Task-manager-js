# Task Manager

A simple Node.js and Express-based REST API for managing tasks, using MongoDB for data storage.

## Features

- Create, read, update, and delete tasks
- RESTful API endpoints
- MongoDB integration with Mongoose

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [MongoDB](https://www.mongodb.com/) running locally or accessible remotely

## Installation

1. Clone the repository:
   ```sh
   git clone <your-repo-url>
   cd Task\ manager
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

3. Start MongoDB if not already running:
   ```sh
   mongod
   ```

## Usage

### Development

Start the server with automatic restarts:
```sh
npm start
```

### Production-like

Start the server without automatic restarts:
```sh
npm run dev
```

The server will run at [http://localhost:3000](http://localhost:3000).

## API Endpoints

| Method | Endpoint         | Description           |
|--------|------------------|-----------------------|
| POST   | `/tasks`         | Create a new task     |
| GET    | `/tasks`         | Get all tasks         |
| GET    | `/tasks/:id`     | Get a task by ID      |
| PUT    | `/tasks/:id`     | Update a task by ID   |
| DELETE | `/tasks/:id`     | Delete a task by ID   |

## Project Structure

```
Task manager/
├── server.js
├── routes.js
├── task.js
├── package.json
├── .gitignore
```

## License

ISC

---

**Note:**  
Make sure MongoDB is running and accessible at `mongodb://localhost:27017/taskdb` or update the connection string in `server.js` as needed.
