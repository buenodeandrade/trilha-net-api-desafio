# DIO - .NET Track - API and Entity Framework
www.dio.me

## Project Challenge
For this challenge, you will need to use the knowledge acquired in the API and Entity Framework module of the DIO .NET track.

## Context
You need to build a task management system where you can register a list of tasks to better organize your routine.

This task list needs to have a CRUD, that is, it should allow you to retrieve, create, save, and delete these records.

Your application should be either a Web API or MVC; feel free to implement the solution you find most appropriate.

Your main class, the task class, should be as follows:

![Task Class Diagram](diagrama.png)

Don't forget to generate your migration to update the database.

## Expected Methods
You are expected to create your methods as follows:

**Swagger**

![Swagger Methods](swagger.png)

**Endpoints**

| Verb   | Endpoint                | Parameter | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Task/{id}              | id        | N/A           |
| PUT    | /Task/{id}              | id        | Task Schema   |
| DELETE | /Task/{id}              | id        | N/A           |
| GET    | /Task/GetAll            | N/A       | N/A           |
| GET    | /Task/GetByTitle        | title     | N/A           |
| GET    | /Task/GetByDate         | date      | N/A           |
| GET    | /Task/GetByStatus       | status    | N/A           |
| POST   | /Task                   | N/A       | Task Schema   |

This is the Task schema (model) used to pass to methods that require it:

```json
{
  "id": 0,
  "title": "string",
  "description": "string",
  "date": "2022-06-08T01:31:07.056Z",
  "status": "Pending"
}
```


## Solution
The code is halfway done, and you should continue it according to the rules described above so that in the end, we have a functional program. Look for the commented word "TODO" in the code, then implement it according to the above rules.
