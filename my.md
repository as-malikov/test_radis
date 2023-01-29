Do migration
```bash
docker-compose run --rm web-app sh -c "python manage.py migrate"
```

Created users in DB
```bash
docker-compose run --rm web-app sh -c "python manage.py createsuperuser"
```

Create object
```bash
docker-compose run --rm web-app sh -c "python manage.py startapp clients"
```

Make migration for object
```bash
docker-compose run --rm web-app sh -c "python manage.py makemigrations clients"
```

Apply migrations
```bash
docker-compose run --rm web-app sh -c "python manage.py migrate clients"
```