# Задание 2. Реализация REST API

## Требования

- В домашнем задании должна быть использовать последняя актуальная (на момент выполнения) версия фреймворка.

## Предыстория

Практически все современные веб приложения используют REST API, поэтому очень важно научиться настраивать его.

## Техническое задание

1. Установите [Laravel Sanctum](https://laravel.com/docs/10.x/sanctum) в свой проект.
2. Создать роут `POST: /api/tokens/create` для выпуска новых токенов.
3. Создать роут `GET: /api/user` по которому будет происходить вывод всей информации об авторизованном пользователе.
4. С помощью **artisan** сгенерировать модель, миграцию и ресурсный контроллер для сущности **cars**, каждая запись 
в БД должна иметь следующую структуру данных:

```php
[
    'id' => 1,
    'brand' => 'Volvo',
    'model' => 'XC90',
    'price' => '4000000',
    'created_at' => '2021-01-22 19:45:07',
    'updated_at' => '2021-01-22 19:45:07',
]
```

Типы данных привести в соответствие с хранимой информацие.

5. Подготовить защищенный `Route::apiResource` для контроллера **CarController** с реализацией всех api-методов.
