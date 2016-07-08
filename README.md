# docker-django
Basic enviroment django

Run the commands:

```sh
docker pull albovieira/docker-django
docker-compose run web django-admin.py startproject myproject .
```

Change the line command in docker-compose file:

```sh
command: bash -c "python manage.py runserver 0.0.0.0:8000 && python manage.py startapp myapp"
```
'myapp' should be changed with the name of your app.

```sh
docker-compose up
```
