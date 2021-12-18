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
2. clone this repo as a submodule by doing ``` git submodule add git@github.com:MomenMuhammad/laravel-docker.git docker ```
3. Go to the submodule folder ``` cd docker ```
4. create new .env file by copying the .env.example ```cp .env.exmpale .env```
5. edit the .env as you like
6. run ```docker-compose up -d```
