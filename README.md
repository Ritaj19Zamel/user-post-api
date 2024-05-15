# User Management and Post API

This repository contains the source code for an API designed for managing user registration, login, and user information management. Additionally, it provides functionality for creating, editing, and retrieving posts associated with users.

## Features

- **User Registration and Login:** Endpoints for user registration and authentication.
- **User Information Management:** Endpoints for retrieving, updating, and adding user information such as name, job title, salary, department, etc.
- **Post Management:** Endpoints for creating, editing, and retrieving posts associated with users.


### User Registration and Login

- `POST /Auth/Register`: Register a new user.
- `POST /Auth/Login`: Authenticate and login a user.
- `POST /Auth/ResetPassword`: Reset password for user.

### User Information Management

- `GET /UserComplete/GetUsers/:id:active`: Retrieve user information by ID.
- `PUT /UserComplete/UpsertUser/:id`: Update or Add user information.
- `DELETE /UserComplete/DeleteUser`: Delete user information.

### Post Management

- `GET /post/Posts/:id:userid:searchparam`: Retrieve post by ID or User ID or Word.
- `GET /Post/MyPosts`: Retrieve post of current User.
- `PUT /Post/UpsertPost`: Update or Add post.
- `DELETE /Post/Post/:id`: Delete Post.

## Usage

To run the API and access the Swagger documentation:

1. Clone this repository to your local machine.
2. Open PowerShell or any terminal of your choice in the location of the solution.
3. Type `dotnet run` or `dotnet watch run` and press Enter.
4. Open your web browser and navigate to `https://localhost:<port>` (by default, Swagger UI runs on port 5001).
5. You should see the Swagger documentation where you can try out all the API endpoints.
