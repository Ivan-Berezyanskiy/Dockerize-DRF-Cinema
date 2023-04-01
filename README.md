# Dockerize-DRF-Cinema
___
- Api service for cinema management written on DRF

## Installing using GitHub:
___
-Install PostgreSQL and create DB

```shell
git clone https://github.com/Vanya2389/Dockerize-DRF-Cinema.git
cd Dockerize-DRF-Cinema
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
Create .env file(You can see how create .env file in .env.sample) 
```
python manage.py migrate
python manage.py runserver
```

## Run with Docker:
___
- Docker should be installed
```
- docker-compose build
- docker-compose up
```

## Getting access:
___
- Create user via /api/user/register/
- Get  token via /api/user/token/
- Authorize with it on /api/doc/swagger/

## Feauters:
___
- JWT authenticated
- Admin panel /admin/
- Documentation is located via /api/doc/swagger/
- Managing orders and tickets
- Media files on movie image (stored in docker)
- Creating movies with actors, genres 
- Filtering movies and movie sessions
