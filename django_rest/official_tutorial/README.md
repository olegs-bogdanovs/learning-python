### Install requirements:
```
pip install -r requirements.txt
```

### Database configuration:

```
docker run -d --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=secret -e POSTGRES_USER=user postgres
createdb -E UTF-8 -h 127.0.0.1 -p 5432 -U user --password database
```

### Database migration:
```
python manage.py migration
python manage.py createsuperuser
```