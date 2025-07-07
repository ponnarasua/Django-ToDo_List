
# 📝 ToDo Web Application

A minimalist and responsive web-based ToDo application built using Django (backend) and HTML/CSS (frontend). This app helps users manage their tasks with deadlines and descriptions.

## 🌐 Live Demo

🔗 [Try it Live on Render](https://todo-list-up2x.onrender.com)

## 📁 Project Structure


TodoApp/
├── todo\_project/         # Django project directory
│   ├── settings.py       # Django settings
│   ├── urls.py           # URL routing
│   └── wsgi.py
├── todo/                 # Django app for ToDo logic
│   ├── models.py         # Task model
│   ├── views.py          # Logic to render/add/delete tasks
│   ├── forms.py          # Task form
│   ├── templates/
│   │   └── todo/
│   │       ├── index.html
│   │       └── edit\_todo.html
├── static/               # Static files (CSS, images)
├── db.sqlite3            # SQLite database
└── manage.py             # Django project manager


## ⚙️ Features

- ✅ Add new tasks with title, description, and due date  
- 📝 Edit existing tasks  
- 🗑 Delete tasks when done  
- 📅 Task deadline support  
- 🎨 Simple, responsive UI with Bootstrap

## 🚀 Getting Started

### 1. Clone the Repository

git clone https://github.com/your-username/todo-django-app.git
cd todo-django-app


### 2. Create Virtual Environment

```bash
python -m venv env
env\Scripts\activate  # On Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Start the Development Server

```bash
python manage.py runserver
```

Go to `http://127.0.0.1:8000/` in your browser.

## 📦 Requirements

* Python 3.10+
* Django 5.2.4
* Bootstrap 5 (CDN)

## 👨‍💻 Contributors

* **Ponnarasu A**

## 📄 License

This project is open-source and free to use for educational and personal purposes.

Let me know if you want to add:
- Screenshots section
- Deployment instructions for Render
- A GitHub badge or live preview iframe

