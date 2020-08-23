# laravel-note

## Cache Clear

```bash
php artisan route:clear
php artisan config:clear
php artisan cache:clear
php artisan view:clear
```

## RESTFUL JSON API

### Notes

- use [Fractal](https://fractal.thephpleague.com) library for Laravel 5.4 and under.
- use Resource Class (introduced in Laravel 5.5)
- `withoutWap()` to un-warp with `data` key
- `$collection->flapMap($callback($value))` to map collection relationship.
- `$collection->map($callback($value))` to map item relationship.

### Resources

- [Using Laravel 5.5 Resources to create your own {JSON:API} formatted API | Laravel 5.5 | by Dean Tedesco | Zero Equals False | Medium](https://medium.com/zero-equals-false/using-laravel-5-5-resources-to-create-your-own-json-api-formatted-api-2c6af5e4d0e8)

## Test Driven Development(TDD)

### Resources

- [Simple TDD in Laravel with 11 steps | by Jeff Simons Decena | Medium](https://medium.com/@jsdecena/simple-tdd-in-laravel-with-11-steps-c475f8b1b214)

## Other Resources

### laravel/passport setup

https://medium.com/techcompose/create-rest-api-in-laravel-with-authentication-using-passport-133a1678a876

### Laravel 6/7 Validation

https://appdividend.com/2019/09/21/laravel-6-validation-example-validation-in-laravel-tutorial/

### PDF Export in Laravel

[Laravel PDF - Create and Download Pdf In Laravel 5.7](https://www.tutsmake.com/laravel-pdf-create-and-download-pdf-file-in-laravel-5-7/)

### Dockerize Laravel App

[Dockerizing Laravel with Nginx MySQL and Docker Compose on Ubuntu 18.04 LTS](https://www.howtoforge.com/dockerizing-laravel-with-nginx-mysql-and-docker-compose/)

### Unit Test AIP in Laravel

https://medium.com/@mscherrenberg/unit-testing-your-api-in-laravel-5-6-7172bcdc593d
https://medium.com/@DCzajkowski/testing-laravel-authentication-flow-573ea0a96318

### Mobile Detect Lib

https://github.com/serbanghita/Mobile-Detect
