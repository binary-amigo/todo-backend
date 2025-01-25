# Task Management Backend

This repository contains the backend for the Task Management App. It provides APIs for managing tasks, including viewing, creating, updating, and deleting tasks. The backend is built using Node.js and MongoDB.

## Features
- API endpoints to create, retrieve, update, and delete tasks.
- Connects to a MongoDB database for task storage.
- Configurable with environment variables (e.g., port, MongoDB URI).

## Technologies Used
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Environment Variables**: `.env` for configuration

## How to Set Up Locally

### Prerequisites
- [Node.js](https://nodejs.org/) (version 12 or above)
- [npm](https://www.npmjs.com/)
- [MongoDB](https://www.mongodb.com/try/download/community) or a cloud MongoDB instance (like MongoDB Atlas)

### Steps to Set Up

1. Clone the repository:
   ```bash
   git clone https://github.com/binary-amigo/todo-backend.git
   ```

2. Navigate to the project directory:
   ```bash
   cd todo-backend
   ```

3. Install the dependencies:
   ```bash
   npm install
   ```

4. Create a `.env` file:
   - In the root directory of the project, create a `.env` file.
   - Add the following configuration:
     ```
     PORT=3000
     MONGODB_URI=mongodb://localhost:27017/todoapp
     ```
     - Replace `mongodb://localhost:27017/todoapp` with your own MongoDB URI if you're using a cloud-based database like MongoDB Atlas.

5. Run the backend server:
   ```bash
   npm start
   ```

6. The server will be running at `http://localhost:3000` (or the configured `PORT` in your `.env` file).

## Endpoints

The following API endpoints are available:

- **GET /tasks**: Retrieve all tasks.
- **POST /tasks**: Create a new task.
- **GET /tasks/:id**: Retrieve a task by ID.
- **PUT /tasks/:id**: Update a task by ID.
- **DELETE /tasks/:id**: Delete a task by ID.
