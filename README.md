# About

Dockerize laravel app for development with nginx, php ,mysql and phpmyadmin



# Run the server :

to run the server you only need to run the **server** service, witch depends on php,mysql,phpmyadmin services.

composer,artisan and npm services are not required to start the server , you can run them independently when you need them

```
docker compose run -d --build server
```

* laravel App : http://localhost:8000

![](images/laravel.png)

* phpmyadmin : http://localhost:8080/

![](images/phpmyadmin.png)


* MYSQL_DATABASE=laravel
* MYSQL_ROOT_PASSWORD=thepassword


# Stop the server :

```
docker compose down
```



# Composer :

To create a new laravel project or install any dependency

```
docker compose run --rm composer create-project laravel/laravel

docker compose run --rm composer require ....
```

# Artisan :

```
docker compose run --rm artisan migrate
```
