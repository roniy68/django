# Django Docked

## Local Development Setup

```
docker compose up 
chmod +x config.sh && ./config.sh
docker compose run --rm app sh -c "python manage.py createsuperuser"

```

### Create Your Django Admin with docker-compose 

```
docker compose run --rm app sh -c "django-admin startproject app ."

```

### Create the core app 

```
docker compose build
docker compose run --rm app sh -c "python manage.py startapp core"

```

### make migrations 

```
docker compose run --rm app sh -c "python manage.py makemigrations"
```

### Admin user creation

```
docker compose run --rm app sh -c "python manage.py createsuperuser"
```

