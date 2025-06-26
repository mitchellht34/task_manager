# README.md

## Task Manager / To-Do List Application

This is a Django-based web application that allows users to manage daily tasks. Users can create, view, edit, mark complete/incomplete, and delete tasks through a clean and responsive interface.

---

### 🚀 Features
- Add new tasks
- Edit existing tasks
- Delete tasks
- Mark tasks as complete or incomplete
- View task list with due dates and statuses

---

### 🛠️ Tech Stack
- **Backend**: Django (Python)
- **Database**: SQLite
- **Frontend**: HTML, CSS, Bootstrap 5

---

### 📁 Project Structure
```
tasksite/           # Django project folder
├── tasksite/       # Project settings
│   ├── settings.py
│   └── urls.py
├── tasks/          # App folder
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│   └── templates/tasks/
│       ├── base.html
│       ├── index.html
│       └── task_form.html
├── db.sqlite3
└── manage.py
```

---

### ⚙️ Setup Instructions
1. **Clone the repo**
    ```bash
    git clone https://github.com/mitchellht34/task_manager
    cd task_manager
    ```
2. **Create and activate a virtual environment**
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use 
    .\env\Scripts\activate # On Mac use
    ```
3. **Install dependencies**
    ```bash
    pip install django
    ```
4. **Apply migrations**
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```
5. **Run the server**
    ```bash
    python manage.py runserver
    ```
6. **Visit in browser**: http://127.0.0.1:8000/

---

### 🗃️ Database Schema
Each Task has:
- `title` (CharField)
- `description` (TextField, optional)
- `due_date` (DateField, optional)
- `is_completed` (BooleanField)

---