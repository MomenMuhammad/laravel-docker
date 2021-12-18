![Issues](https://img.shields.io/github/issues/MomenMuhammad/laravel-docker)
![Issues](https://img.shields.io/github/forks/MomenMuhammad/laravel-docker)
![Issues](https://img.shields.io/github/stars/MomenMuhammad/laravel-docker)
# Basic Docker Environment For Laravel
Basic Docker Configuration for laravel project

# Docker Images Included
- php:8.0.8-apache
- elasticsearch:7.13.3
- mysql:8.0.25
- redis:6.2.4

# Steps
1. Go to your project 
2. clone this repo as a submodule by doing ```git submodule add git@github.com:MomenMuhammad/laravel-docker.git docker```
3. Go to the submodule folder ```cd docker```
4. create new .env file by copying the .env.example ```cp .env.exmpale .env``` for more information about [ENV variables](#env-variables-description)
5. edit the .env as you like
6. run ```docker-compose up -d```

# ENV variables description
## MySQL Variables
- ```MYSQL_EXTERNAL_PORT ``` : External mysql port number (outside the contrainer)
- ```MYSQL_INTERNAL_PORT ``` : Internal mysql port number (inside the container)
- ```MYSQL_DATABASE_FILES_PATH ``` : Database files location in your machine
- ```MYSQL_DATABASE_PATH ``` : sql files location in your machine to run for the first time
- ```MYSQL_USERNAME``` : database's username
- ```MYSQL_PASSWORD``` : database's password
- ```MYSQL_DATABASE``` : database's name
- ```MYSQL_ROOT_PASSWORD``` : database's root's password
- ```MYSQL_ROOT_PASSWORD``` : database's root's password
- ```MYSQL_CONTAINER_NAME``` : mysql container name
## Apache PHP (APPLICATION)
- ```APPLICATION_INTERNAL_HTTP_PORT``` : Internal HTTP Apache port (inside the container)
- ```APPLICATION_EXTERNAL_HTTP_PORT``` : External HTTP Apache port (outside the container)
- ```APPLICATION_EXTERNAL_HTTPS_PORT``` : External HTTPS Apache port (outside the container)
- ```APPLICATION_INTERNAL_HTTPS_PORT``` : Internal HTTPS Apache port (inside the container)
- ```APPLICATION_CONTAINER_NAME``` : Apache PHP container name
## ELASTICSEARCH
- ```ELASTICSEARCH_EXTERNAL_REQUEST_PORT``` : External request port (outside the container)
- ```ELASTICSEARCH_INTERNAL_REQUEST_PORT``` : Internal HTTP Apache port (inside the container)
- ```ELASTICSEARCH_EXTERNAL_COMMUNICATION_PORT``` : External Communication port (outside the container)
- ```ELASTICSEARCH_INTERNAL_COMMUNICATION_PORT``` : Internal Communication port (inside the container)
- ```ELASTICSEARCH_CONTAINER_NAME``` : Elasticsearch container name
## REDIS
- ```REDIS_EXTERNAL_REDIS_PORT``` : External Redis port (outside the container)
- ```REDIS_INTERNAL_REDIS_PORT``` : Internal Redis port (inside the container)
- ```REDIS_CONTAINER_NAME``` : Redis container name
## Global DOCKER
- ```NETWORK_NAME``` : Global Docker Network Name