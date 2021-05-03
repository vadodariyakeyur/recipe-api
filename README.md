# Recipe REST API
## **Made with:**  

<img src="https://wallpapersfortech.com/?attachment_id=13195" alt="Python Logo" height="200"/> <img src="https://soshace.com/wp-content/uploads/2021/01/879-png-3.png" alt="Django + Django REST Framework Logo" height="200"/>

\
<img src="https://techcrunch.com/wp-content/uploads/2015/09/docker-dark.png?w=1390&crop=1" height="200"/>
<img src="https://miro.medium.com/max/1600/0*cYz18RKjh72UZdN-.png" height="200"/>
<img src="https://cdn-bhdil.nitrocdn.com/isrDVIFCpCXbHHPoNruCoFKRiVumSNxS/assets/static/optimized/wp-content/uploads/6474aa16a99e8d32db4e89bdabbb2807.postgresql-connection-refused-298x300.png" height="200"/>

- - - - 

## To set up project ##
```sh
$ docker-compose build
```

- - - - 

## Run all tests ##
```sh
$ docker-compose run --rm app sh -c "bash ./wait-for-postgres.sh db 5432 python manage.py test && flake8"
```

- - - - 

## Run API server ##
```sh
$ docker-compose up
```

- - - - 

## Create superuser

```sh
$ docker-compose run app sh -c "python manage.py createsuperuser"
Email address: admin@example.com
Password: **********
Password (again): *********
Superuser created successfully.
```
