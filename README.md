# Laravel Hands-on Assignment

## Duration: 2 Hours

### Task:
You have to create a Task Management API using Laravel. Complete the following tasks by implementing them in your Laravel project.

1. **Laravel Project Setup**
    - Create a new Laravel project.

2. **Database & Migrations**
    - Create a `tasks` table using Laravel migrations with the following fields:
      - `id` (Auto-increment)
      - `title` (String)
      - `description` (Text, nullable)
      - `status` (Enum: pending/completed, default: pending)
      - `due_date` (Date)
      - `timestamps` (Laravel default)
    - Provide the Laravel migration file for this table.

3. **Eloquent Model**
    - Create a `Task` model in Laravel.
    - Define its fillable properties.

4. **RESTful API Endpoints**
    - Create a `TaskController` and implement the following API routes:
      - `GET /api/tasks` -> Fetch all tasks
      - `POST /api/tasks` -> Create a new task
      - `GET /api/tasks/{id}` -> Fetch a single task
      - `PUT /api/tasks/{id}` -> Update a task
      - `DELETE /api/tasks/{id}` -> Delete a task
    - Provide the controller code implementing these CRUD operations.

5. **Validation & Error Handling**
    - Implement request validation for creating and updating tasks.
    - Ensure that `title` is required and `due_date` is a valid date.
    - Provide the validation rules in your controller.
