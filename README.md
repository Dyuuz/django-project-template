# Django Project Template

A reusable, production-ready **Django project template** designed to help you start new projects fast — without creating a Django project from scratch every time.

This template is opinionated but flexible, suitable for APIs, dashboards, and full-stack Django applications.

---

## ✨ Features

- Pre-configured Django project structure
- Environment variable support via `.env`
- Works with:
  - Virtual environments
  - `requirements.txt`
  - Docker
- Ready for extension with Django REST Framework, auth, and more
- Open-source and fork-friendly

---

## 📁 Project Structure

```text
.
├── manage.py
├── basekit/                 # Main Django settings module
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
├── apps/                 # Create Django apps
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── .env.example
└── README.md

## 🚀 Getting Started

You can either **fork** or **clone** this repository to start a new Django project without running `django-admin startproject`.

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

## Virtual Environment (Required)

You must create and activate a virtual environment manually.

```Windows

```
python -m venv venv
venv\Scripts\activate
```

```Linux/macOS

```
python3 -m venv venv
source venv/bin/activate
```

## Install Dependencies

```
pip install -r requirements.txt
```

## .env format

```
SECRET_KEY=''
DEBUG=True
ALLOWED_HOSTS='localhost,127.0.0.1'
CSRF_TRUSTED_ORIGINS=''
CORS_ALLOWED_ORIGINS=''
```

## ⚠️ Important Notes

SECRET_KEY must be set before running in production

CSRF_TRUSTED_ORIGINS and CORS_ALLOWED_ORIGINS must include a valid scheme (http:// or https://)

Do not commit your .env file

## 🗄️ Database Setup

```
python manage.py migrate
```

## ➕ Creating a New App

```
python manage.py startapp myapp
```

## ⭐ Support

If you find this template useful, consider starring the repo 🌟

