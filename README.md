# Django Translator App - Installation Guide

## 🛠 Prerequisites
Ensure you have **Python** installed on your system before proceeding.

## 🚀 Installation Steps

### 1️⃣ Clone the Repository  
You can clone the repository using HTTPS or SSH:

#### Clone using HTTPS:
```sh
git clone https://github.com/Venkat-Kowshik/FAQ.git  
cd FAQ  
```

#### Clone using SSH:
```sh
git clone git@github.com:Venkat-Kowshik/FAQ.git  
cd FAQ  
```

### 2️⃣ Create a Virtual Environment  
Before installing dependencies, it is recommended to create a virtual environment:

```sh
python -m venv venv  
source venv/bin/activate  # On macOS/Linux  
venv\Scripts\activate  # On Windows  
```

### 3️⃣ Install Django & Translate Package  
```sh
pip install django translate  
```

### 4️⃣ Create & Setup Django Project  
```sh
django-admin startproject translator  
cd translator  
python manage.py startapp app  
```

### 5️⃣ Add the App to INSTALLED_APPS  
Modify **settings.py**:  

```python
INSTALLED_APPS = [  
    "django.contrib.admin",  
    "django.contrib.auth",  
    "django.contrib.contenttypes",  
    "django.contrib.sessions",  
    "django.contrib.messages",  
    "django.contrib.staticfiles",  
    "app",  # New App  
]
```

### 6️⃣ Run the Server  
Once everything is set up, start the Django server:  

```sh
python manage.py runserver  
```

Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) to use the app.
