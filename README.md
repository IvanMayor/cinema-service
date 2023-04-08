# Cinema API

API service for cinema management written on DRF

## Features:
 
- JWT authenticated
- Admin panel /admin/
- Documentation is located /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

## Installing using GitHub:

### Install PostgresSQL and create db

- Clone repository by command:
```
git clone https://github.com/IvanMayor/cinema-service.git
```
- Change directory:
```
cd cinema-service
```
- Crete virtualenv:
```
python -m venv venv
```
- Activate virtualenv:
```
venv/Scripts/activate
```
- Install requirements:
```
pip install -r requirements.txt
```
- Set environ variables
```
set POSTGRES_HOST=<your db hostname>
set POSTGRES_DB=<your db name>
set POSTGRES_USER=<your db username>
set POSTGRES_PASSWORD=<your db password>
set SECRET_KEY=<your secret key>
```
- Run migrations:
```
python manage.py migrate
python manage.py runserver
```

## Run by docker:

### Docker should be installed

```
docker-compose build
docker-compose up
```
## Getting access

- create user /api/user/register/
- get access token /api/user/token/
