# CampusConnect

A Django web application for campus community management, built for **CSIT327**. Users can sign up, log in, view a personalized dashboard, and (for admins) access an admin panel.

## Features

- User registration and login with a custom user model
- Role-based access (Admin, Staff, User)
- Personalized dashboard showing role, course, member count, and last login
- Admin-only panel protected by `LoginRequiredMixin` and `UserPassesTestMixin`
- Responsive UI styled with Bootstrap 5

## Tech Stack

- Python 3
- Django
- SQLite (default database)
- Bootstrap 5 (via CDN)

## Project Structure

```
campusconnect/
├── accounts/          # Custom user model, sign up, login
├── dashboard/         # Dashboard and admin panel views
├── campusconnect/     # Project settings and root URLs
├── templates/         # Shared templates (base.html)
└── manage.py
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/KarlManzalinto/CSIT327-G5-Manzalinto-Karl-FirstDjango.git
cd CSIT327-G5-Manzalinto-Karl-FirstDjango
```

### 2. Create and activate a virtual environment

```bash
python -m venv .venv
.venv\Scripts\activate        # Windows
source .venv/bin/activate     # macOS / Linux
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Apply migrations

```bash
python manage.py migrate
```

### 5. (Optional) Create a superuser

```bash
python manage.py createsuperuser
```

### 6. Run the development server

```bash
python manage.py runserver
```

Open http://127.0.0.1:8000/ in your browser.

## Usage

| Page        | URL            | Access               |
|-------------|----------------|----------------------|
| Dashboard   | `/`            | Logged-in users      |
| Admin panel | `/admin-panel/`| Users with Admin role|
| Sign up     | `/signup/`     | Everyone             |

## Author

**Karl Manzalinto**
CSIT327 | Group 5

## License

This project was created for academic purposes.
