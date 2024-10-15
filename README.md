# To-Do Application

## Overview
A simple task management web application built with Django, allowing users to register, log in, and manage their daily tasks. Users can add, update, and delete tasks, and track their completion status.

## Features
- **User Authentication**: Users can register, log in, and log out securely.
- **Task Management**: Add, update, delete, and mark tasks as completed.
- **User-Specific Dashboard**: Each user sees only their tasks.
- **Responsive Design**: Frontend built with Bootstrap for a mobile-friendly experience.
- **Admin Panel**: Manage users and tasks through the Django admin interface.

## Technologies Used
- **Backend**: Django (Python)
- **Database**: SQLite (Django ORM)
- **Frontend**: HTML, CSS, Bootstrap
- **Version Control**: Git

## Installation

### Prerequisites
- Python 3.x installed on your machine.
- Django framework installed (`pip install django`).

### Steps to Run Locally

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/todo-app.git
    cd todo-app
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run migrations to set up the database:
    ```bash
    python manage.py migrate
    ```

4. Create a superuser for the admin panel:
    ```bash
    python manage.py createsuperuser
    ```

5. Start the development server:
    ```bash
    python manage.py runserver
    ```

6. Access the app by navigating to `http://127.0.0.1:8000/` in your web browser.

### Admin Panel
To access the Django admin panel, visit `http://127.0.0.1:8000/admin` and log in using the superuser credentials.

## Usage

1. **Register** a new user or log in with an existing account.
2. On the **Dashboard**, add new tasks, mark tasks as completed, update, or delete tasks.
3. Log out once done managing tasks.

## Project Structure
```
|-- todoprj/
    |-- manage.py
    |-- todoprj/
    |   |-- settings.py
    |   |-- urls.py
    |   |-- wsgi.py
    |-- todoapp/
        |-- migrations/
        |-- templates/
        |   |-- todoapp/
        |       |-- login.html
        |       |-- register.html
        |       |-- todo.html
        |-- admin.py
        |-- models.py
        |-- views.py
        |-- urls.py
```

## Security Considerations
- Passwords are hashed using Django’s built-in password hashing system.
- User sessions are handled securely using Django’s session framework.
- CSRF protection is enabled by default.

## Future Improvements
- **Task Prioritization**: Allow users to set priorities for their tasks.
- **Due Dates**: Add an option to assign due dates to tasks.
- **API Integration**: Expose a REST API for task management.
