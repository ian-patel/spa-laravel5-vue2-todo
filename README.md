[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b92fb0f13fd440a1a50dd7cfcc2d27df)](https://www.codacy.com/app/ian-patel/spa-laravel5-vue2-todo?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ian-patel/spa-laravel5-vue2-todo&amp;utm_campaign=Badge_Grade)

# Dockerized Laravel & Vue.js TODO application

Docker running Nginx, PHP, Composer and MySQL.

## Overview

1. [Install prerequisites](#install-prerequisites)

    Before installing project make sure the following prerequisites have been met.

2. [Clone the project](#clone-the-project)

    We’ll download the code from its repository on GitHub.

5. [Setup the application](#setup-the-application)

    By this point we’ll have all the project pieces in place.

6. [Start/stop the application](#start-the-application)


7. [Useful commands](#useful-commands)

   

___

## Install prerequisites

For now, this project has been mainly created for Unix `(Linux/MacOS)`. Perhaps it could work on Windows.

All requisites should be available for your distribution. The most important are :

* [Git](https://git-scm.com/downloads)
* [Docker](https://docs.docker.com/engine/installation/)
* [Docker Compose](https://docs.docker.com/compose/install/)

Check if `docker-compose` is already installed by entering the following command :

```sh
which docker-compose
```

Check Docker Compose compatibility :

 - [Compose file version 3 reference](https://docs.docker.com/compose/compose-file/)

The following is optional but makes life more enjoyable :

```sh
which make
```

## Clone the project

To install [Git](http://git-scm.com/book/en/v2/Getting-Started-Installing-Git), download it and install following the instructions :

```sh
git clone https://github.com/ian-patel/spa-laravel5-vue2-todo.git
```

Go to the project directory :

```sh
cd spa-laravel5-vue2-todo
```

---

## Setup the application

1. Run this magic command

    ```sh
    make setup
    ```

2. Migrate database

	 ```sh
    make setup-database



---

## Start the application

Start the application using docker

```sh
make docker-start
``` 
    
 Application is ready on localhost 8003 port.
    
    http://localhost:8003/
    

---
## Stop the application

Stop the application using docker

```sh
make docker-stop
``` 
    

---


## Useful commands

PHPUnit test

```sh
make phpunit
```

List artisan commands :

```sh
make artisan
```

Start artisan tinker :

```sh
make tinker
```


#### Connecting MySQL


```php
host:     127.0.0.1
port:     33063
database: todo
username: who
password: what
```

---


Developed by [@patel_ian](https://twitter.com/patel_ian)