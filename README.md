# Django Login Application

A secure Django authentication system with email verification, password reset, and user dashboard.

## Features

- User Registration (Signup)
- Email Verification
- Secure Login/Logout
- Password Reset (optional)
- User Dashboard
- Bootstrap UI

## Installation

### Prerequisites
- Python 3.8+
- MySQL Server
- Git

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/shIhab-md-akash/login203.git
   cd login203
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Create `.env` file**
   ```
   DEBUG=True
   SECRET_KEY=your-secret-key-here
   DATABASE_NAME=login_db
   DATABASE_USER=root
   DATABASE_PASSWORD=your-password
   ```

5. **Run migrations**
   ```bash
   python manage.py migrate
   ```

6. **Create superuser**
   ```bash
   python manage.py createsuperuser
   ```

7. **Start server**
   ```bash
   python manage.py runserver
   ```

Access the app at `http://127.0.0.1:8000/`

## Project Structure

```
login203/
├── login/                 # Main project settings
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── loginapp/             # Main Django app
│   ├── views.py
│   ├── urls.py
│   ├── models.py
│   └── templates/
│       └── loginapp/
│           ├── base.html
│           ├── login.html
│           ├── signup.html
│           └── dashboard.html
├── static/              # CSS, JS, images
├── media/               # User uploads
├── manage.py
└── requirements.txt
```

## URLs

- `/` - Home (redirects to login)
- `/login/` - User Login
- `/signup/` - User Registration
- `/logout/` - User Logout
- `/dashboard/` - User Dashboard
- `/admin/` - Admin Panel

## Technology Stack

- **Backend**: Django 4.2
- **Database**: MySQL
- **Frontend**: Bootstrap 5
- **Email**: Django Email Backend

## Author

Shihab Md. Akash

## License

MIT