### Easyest way to connect PG database

- Create `VENV` and run that machine
- Install django
  ```bash
  python -m pip install Django
  ```
  - Check the django installed version
  ```bash
  django-admin --version
  ```
- Create **`django`** project
  ```bash
  django-admin startproject project_name
  ```
- Install `psycopg2`
  ```bash
  pip install psycopg2
  ```
- Put your DB data source

```py
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql',
            'NAME': "djangodb",
            'USER': "djangodb_owner",
            'PASSWORD': "M6BKoWYGgCt4",
            'HOST': "ep-floral-sun-a1n5ny2c.ap-southeast-1.aws.neon.tech",
            'PORT': "5432",
            'OPTIONS': {
                'sslmode': 'require',
            },
        }
    }
```

- Run `django` project
  ```bash
  python manage.py runserver
  ```
