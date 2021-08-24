# Task Manager API
Task manager application built using node.JS and MongoDB. It follows a RESTFul API design architecture.
The app sends an email notification upon registration and deactivation of the user's account.
Each user, affter login can add new tasks, mark them as completed and sorting, pagination and filtering them.

# Main features

* Sending emails
* Authentication and security
* Sorting, pagination and filtering
* Uploade profile picture

# API Endpoints

  Methodes    |    Endpoints   | Description   | Access 
------------- | -------------  | ------------- | -------------
POST    | /users | Creat new user  | Public
POST    | /users/login | User login | Public
POST    | /users/logout| Logaout an account | Private
POST    | /users/logoutAll| Logaout all accounts | Private
POST    | /users/me/avatar| Uploade profile picture | Private
POST    | /tasks| Creat new task | Private
GET     | /users/me| User profile  | Private
GET     | /tasks| Shows all my tasks  | Private
GET     | /tasks/tasdId| Shows a single task  | Private
GET     | /tasks?sortBy=createdAt:desc| Sort by Descending order of created date | Private
GET     | /tasks?sortBy=createdAt:asc| Sort by Ascending order of created date | Private
GET     | /tasks?completed=true| Filter by completed task | Private
GET     | /tasks?completed=false| Filter by uncompleted task | Private
GET     | /tasks?limit=2| Limit the result to 2 in a page | Private
GET     | /tasks?skip=3| Paginating result | Private
PATCH   | /users/me| Update user profile | Private
PATCH   | /tasks/taskId| Update a task | Private
DELETE  | /users/me| Delete user profile | Private
DELETE  | /tasks/taskId| Delete a task | Private
DELETE  | /users/me/avatar| Delete user profile picture | Private

