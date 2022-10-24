<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Aprendiendo Laravel

Laravel tiene la [documentación](https://laravel.com/docs) y la biblioteca de tutoriales en video más extensa y completa de todos los marcos de aplicaciones web modernos, por lo que es muy fácil comenzar a usar el marco.

Si no tiene ganas de leer, [Laracasts](https://laracasts.com) puede ayudarlo. Laracasts contiene más de 1500 tutoriales en video sobre una variedad de temas que incluyen Laravel, PHP moderno, pruebas unitarias y JavaScript. Mejore sus habilidades explorando nuestra completa biblioteca de videos.

# Craftable #
## Presentación ##
Hola Crafter es un conjunto de herramientas de código abierto basado en Laravel para crear interfaces de administración. Es una plantilla minimalista de área de administración. Un punto de partida para desarrollar sistemas de back-office, intranets o sistemas CMS.

![Craftable administration area example](https://www.getcraftable.com/docs/5.0/images/posts-crud.png "Craftable administration area example")

Podría llamarlo CMS, pero es muy pequeño, con el menor contenido posible para administrar. Tiene:
- Interfaz de usuario: buena plantilla de administración basada en CoreUI (http://coreui.io/)
- Generador CRUD
- Autorización, Mi perfil y Usuarios CRUD
- Gerente de traducciones
- otros ayudantes para iniciar rápidamente su nueva área de administración (Biblioteca de medios, Lista de administradores, etc.)

- [Requerimientos](#Requerimientos-para-la-ejecución-de-este-proyecto)
- [Instalaciones](#Instalaciones)
  - [Instalación Laravel](#Instación-Laravel)
  - [Instalación Craftable](#Instación-Craftable)
  - [Ejecución](#Ejecución)





# Requerimientos para la ejecución de este proyecto #

requerimientos de Craftable:
- PHP 7.4+
- Supported databases:
  - MySQL 5.7+
  - PostgreSQL 9.5+
- npm 5.3+
- node 8.4+

Craftable uses Laravel so you should check out its requirements too. It is compatible with Laravel 8:
- https://laravel.com/docs/8.x/installation#server-requirements

# Instalaciones #

## Instalación Laravel ##

### Nuevo proyecto laravel 8.0 ###

Instalamos Laravel version 8.0 via Composer

```bash
composer create-project laravel/laravel:^8.0 parcial-app
```

nos situamos en la carpeta del proyecto
```bash
cd parcial-app
```

Actualizamos composer
```bash
composer update
```


## Instalación Craftable ##

### Nuevo proyecto Craftable 7.0 ###


Instalamos el craftable 7.0 via composer:
```bash
composer require brackets/craftable:^7.0 --ignore-platform-req=ext-exif
```

Instalamos admin generator:
```bash
composer require brackets/admin-generator --ignore-platform-req=ext-exif
```

Cree una base de datos vacia y configure en el `.env` (PostgreSQL or MySQL).

Ahora instala el craftable en tu proyecto:
```bash
php artisan craftable:install
```

Actualiza las dependencias:
```bash
npm install --save-dev laravel-mix@latest
```

Instala npm:
```bash
npm install && npm run dev
```
## Ejecuta tu proyecto ##
```bash
php artisan serve
```
