# Student Registration Portal

A Django-based web application to manage student registrations.

---

## 🖥️ Requirements

Make sure the following are installed on your system:

- Python 3.10+  
- pip (Python package manager)  
- PostgreSQL  
- Git (optional, for cloning the repo)

---

## 🚀 Steps to Run Locally

### 1. 📁 Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Student-Registration-Portal.git
cd Student-Registration-Portal
```

> Or download the ZIP file and extract it.

---

### 2. 📦 Create & Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate      # Linux/macOS
# OR
venv\Scripts\activate         # Windows
```

---

### 3. 📥 Install Required Packages

```bash
pip install -r requirements.txt
```

---

### 4. 🛠️ Set Up the Database (PostgreSQL)

Make sure PostgreSQL is running.

Create a database named `studentdb` and update credentials if needed.

In `studentproject/settings.py`, confirm or update:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'studentdb',
        'USER': 'postgres',
        'PASSWORD': '1234',        # ← Change if needed
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

---

### 5. ⚙️ Apply Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

---

### 6. 🧑‍💼 Create Superuser (Optional Admin Login)

```bash
python manage.py createsuperuser
```

---

### 7. 🌐 Run the Development Server

```bash
python manage.py runserver
```

Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

---

## 🧾 Notes

- The main app is `studentapp`.
- Project folder is `studentproject`.
- Made by `Bilal Ilyas Jhandir` for `Web Design & Development Frameworks` Assignment
- Admin dashboard available at `/admin`.
