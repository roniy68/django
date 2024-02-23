# Django Experiment

### Create Your Django app with docker-compose 

```
docker compose run --rm app sh -c "django-admin startproject app ."

```

### Create app 

```
docker compose build
docker compose run --rm app sh -c "python manage.py startapp core"

```