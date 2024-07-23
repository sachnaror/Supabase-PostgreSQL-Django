# Supabase-PostgreSQL-Django

Django-PostgreSQL is a project that demonstrates how to connect a Django application to a PostgreSQL database.

## Prerequisites

- Python 3.12
- Django 5.0
- psycopg2-binary

## Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/Supabase-Django.git
   cd Supabase-Django

2. **Create and activate a virtual environment:**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt

4. **Update settings.py**
   with the PostgreSQL database configuration:
   Open Supabase-Django/settings.py and update the DATABASES configuration:

```bash
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql_psycopg2',
            'HOST': 'aws-34-ap-south-7.pooler.supabase.com',
            'NAME': 'postme',
            'USER': 'postgres.eadfvvbutsqgurzq',
            'PORT': '6973',
            'PASSWORD': 'iE0f4b9yL54M',
        }
    }

5. **Run migrations:**

    ```bash
    python manage.py migrate

6. **Run the development server:**

    ```bash
    python manage.py runserver
