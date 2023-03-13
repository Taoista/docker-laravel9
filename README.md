<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Lravel docker

# Docker Larvel 9 - Vite

Contenedor Docker laravel 9.52 - php 8.1 - Vite

## Instalacion

Clona el repo

```bash
git clone git@github.com:Taoista/docker-laravel9.git
```
Entra al proyecto
```bash
cd docker-laravel9
```

## Uso
Despues descargar, ejecutar

```docker
docker-compose up -d
```
verifica el nombre del contenedor (lo puedes cambiar, deberias)

```bash
CONTAINER ID   IMAGE                     COMMAND                  CREATED          STATUS          PORTS                  NAMES
c2dc66117465   nginx:1.21.6-alpine       "/docker-entrypoint.…"   18 minutes ago   Up 18 minutes   0.0.0.0:8080->80/tcp   webserver
b16a4d34e637   docker-laravel9-backend   "docker-php-entrypoi…"   18 minutes ago   Up 18 minutes   9000/tcp               backend
```
en este caso el container es 'backend', entra en la consola

```bash
docker-compose exec backend sh
```
ejectua

```bash
composer install
```
```bash
npm install
```
```bash
cp .env.example .env
```
```bash
php artisan key:generate
```
si estas trabajando con xampp y/o largon, crea un usuario con los privilegios completos y en la configuracion de mysql agrega
```bash
bind-address=0.0.0.0
```



