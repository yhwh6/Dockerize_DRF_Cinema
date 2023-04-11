# Cinema API
<hr>

API service for cinema management writen on DRF

## Installing using GitHub
<hr>

Install PostgreSQL and create db

```python
git clone https://github.com/yhwh6/Dockerize_DRF_Cinema.git
cd Dockerize_DRF_Cinema

python -m venv venv
source venv/bin/activate

pip install -r requirements.txt
rename .env.sample => .env and insert your data

python manage.py migrate
python manage.py runserver
```

## Run with docker
<hr>

Docker should be installed

```python
docker pull yhwh6/cinema-service
cd cinema-service
docker-compose up
```
Open in browser 127.0.0.1:8000/api/

## Getting access
<hr>

You can use following superuser:
```shell
- Email: admin@test.com
- Password: 1
```

Or create another one by yourself:

- create user via api/user/register/

To work with token use:
- get access token and refresh token via api/user/token/
- verify access token via api/user/token/verify/
- refresh access token via api/user/token/refresh/

## Features:
<hr>

- JWT authenticated
- Admin panel: /admin/
- Documentation is located at: /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres and actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie session

