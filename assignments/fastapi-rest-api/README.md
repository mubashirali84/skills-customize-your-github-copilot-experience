# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with FastAPI to practice defining data models, handling HTTP requests, and returning appropriate responses. Store tasks in memory so you can focus on API behavior rather than database setup.

## 📝 Tasks

### 🛠️ Set Up the API

#### Description
Create a FastAPI application for managing tasks and define the data it will store.

#### Requirements
Completed program should:

- Install FastAPI and Uvicorn and create an application in `main.py`.
- Define a Pydantic model for a task with an integer ID, a title, a description, and a completion status.
- Store tasks in an in-memory collection.
- Provide `GET /tasks` to return all tasks and `GET /tasks/{task_id}` to return one task by ID.
- Return an HTTP 404 response when a requested task ID does not exist.

### 🛠️ Add Task Management Routes

#### Description
Add routes that let clients create, update, and delete tasks using standard HTTP methods.

#### Requirements
Completed program should:

- Provide `POST /tasks` to create a task and return the created task with its assigned ID.
- Provide `PUT /tasks/{task_id}` to update an existing task.
- Provide `DELETE /tasks/{task_id}` to remove an existing task.
- Return an HTTP 404 response when an update or delete request uses an unknown task ID.
- Use Pydantic request models to validate task data and appropriate HTTP status codes for successful requests.

### 🛠️ Test the API

#### Description
Run the application and use FastAPI's interactive documentation to check the routes and their responses.

#### Requirements
Completed program should:

- Start successfully with Uvicorn and make the interactive documentation available at `/docs`.
- Demonstrate creating a task, listing tasks, retrieving one task, updating it, and deleting it.
- Verify that requesting a task with an unknown ID returns HTTP 404.