# Student Portal Web Application

A Django-based Student Portal Web Application designed to digitize and simplify student information management within an educational institution. The system provides a centralized platform for student registration, profile management, document handling, notices, academic information, and administrative operations.

## 📌 Project Overview

The Student Portal replaces traditional manual student record management with a centralized web-based system. Students can register, log in, manage their profiles, view academic information, and access institutional notices, while administrators can manage student records and portal activities.

The application follows Django's **Model-Template-View (MTV)** architecture and uses Django ORM for database interaction. SQLite is used as the default database for development.

## 🚀 Features

### Student Features
- Student registration
- Secure login and authentication
- Personalized student dashboard
- Profile management
- Profile picture upload
- Personal and academic information management
- Document upload and access
- Academic information viewing
- Notice and announcement viewing

### Administrator Features
- Secure admin authentication
- View and manage student records
- Add, edit, and delete student information
- Search, filter, and sort student records
- Manage student profiles
- Publish notices and announcements
- Access Django Admin Panel

The documentation also describes optional academic modules for marks, subject-wise scores, and attendance.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend programming |
| Django | Web application framework |
| HTML | Web page structure |
| CSS | Styling and responsive design |
| JavaScript / jQuery | Optional interactive functionality |
| Django Templates | Dynamic UI rendering |
| SQLite | Development database |
| Django ORM | Database interaction |
| Pillow | Image handling |
| Bootstrap | Optional UI components |

## 🏗️ Architecture

The project follows Django's **MTV (Model-Template-View)** architecture:

- **Model** – Manages application data and database tables.
- **Template** – Handles the presentation layer using HTML/CSS.
- **View** – Processes requests and implements application logic.

### Project Structure

```text
student_portal/
│
├── manage.py
├── db.sqlite3
├── requirements.txt
│
├── student_portal/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
└── students/
    ├── migrations/
    ├── templates/
    │   └── students/
    ├── static/
    ├── admin.py
    ├── apps.py
    ├── models.py
    ├── tests.py
    ├── urls.py
    └── views.py
```

The documented project structure separates configuration, application logic, templates, static files, models, views, and database migrations.

## 💾 Database

The application uses **SQLite** as the default development database. Django ORM is used to define models and interact with the database.

The database is designed to manage information related to:

- Students
- Departments
- Courses
- Student profiles
- Documents
- Notices
- User authentication

For production environments, the documentation suggests using databases such as **PostgreSQL or MySQL** with the appropriate database adapter.

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd student_portal
```

### 2. Create a Virtual Environment

```bash
python -m venv env
```

### 3. Activate the Virtual Environment

**Windows:**

```bash
env\Scripts\activate
```

**Linux/macOS:**

```bash
source env/bin/activate
```

### 4. Install Dependencies

```bash
pip install django
pip install pillow
```

If a `requirements.txt` file is available:

```bash
pip install -r requirements.txt
```

### 5. Apply Database Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Create an Administrator Account

```bash
python manage.py createsuperuser
```

Follow the prompts to enter the username, email, and password.

### 7. Run the Development Server

```bash
python manage.py runserver
```

Open the application in your browser:

```text
http://127.0.0.1:8000/
```

The documentation demonstrates the same Django development-server workflow and provides separate URLs for registration, student records, and the admin panel.

## 🌐 Application URLs

| URL | Purpose |
|---|---|
| `/register/` | Student registration |
| `/students/` | Student list |
| `/admin/` | Django administration panel |

Example:

```text
http://127.0.0.1:8000/register/
http://127.0.0.1:8000/students/
http://127.0.0.1:8000/admin/
```

## 🔐 Authentication & Security

The application uses Django's built-in authentication system.

Security-related functionality includes:

- User authentication
- Password hashing
- Role-based access
- Student-specific profile access
- Administrative access through Django Admin

Students are intended to manage their own information, while administrators have broader permissions to manage student records.

## 🎨 User Interface

The portal is designed with a responsive interface that can be accessed from desktops, tablets, and mobile devices.

The UI uses:

- HTML
- CSS
- Django Templates
- Optional Bootstrap
- Optional JavaScript/jQuery

The documented project output includes login, student registration, admin login, and Django administration screens.

## 🧪 Testing

After starting the development server, the following pages can be tested:

1. **Student Registration**
   - Register a new student.
   - Validate student information.
   - Upload a profile picture.

2. **Student List**
   - View registered student records.

3. **Admin Panel**
   - Log in as an administrator.
   - Add, edit, delete, and manage student profiles.

The project documentation includes screenshots demonstrating the login, registration, admin login, and admin panel interfaces.

## 📋 System Requirements

### Software

- Python 3.8+
- Django 4.x or later
- SQLite
- Modern web browser
- VS Code, PyCharm, or another IDE
- Python virtual environment

### Recommended Hardware

- Quad-core 2.5 GHz processor or higher
- 8 GB RAM or more
- SSD with 50+ GB free space
- Stable internet connection

These requirements are based on the project documentation.

## 🔮 Future Enhancements

Possible future improvements include:

- PostgreSQL/MySQL production database
- Forgot-password and password-reset functionality
- Advanced attendance management
- Marks and grade management
- Subject-wise academic performance
- Improved document management
- Additional student communication features
- Production deployment using Gunicorn and Nginx

## 🎯 Learning Outcomes

This project provides practical experience in:

- Python web development
- Django framework
- MTV architecture
- Django ORM
- Database design
- User authentication
- CRUD operations
- Form handling and validation
- File and image uploads
- Django Admin
- Responsive web interface development

## 📌 Conclusion

The Student Portal Web Application demonstrates how Django can be used to build a modular and secure full-stack web application for educational institutions. By centralizing student information and administrative operations, the system helps streamline academic workflows, reduce manual administrative effort, and improve access to student information.

---

### 👨‍💻 Developer

**Vigneshwaran B**

Bachelor of Engineering – Computer Science and Engineering

**Technologies:** Python • Django • HTML • CSS • JavaScript • SQLite