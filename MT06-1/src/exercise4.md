## Примеры эндпоинтов

Эндпоинт мы будем записывать следующим образом: `{METHOD} /api/{VERSION}/{CLASS}`. 

- METHOD — GET, POST и т.д.
- VERSION — версия API (в нашем случае будем использовать `v1`)
- CLASS — класс объектов, к которому мы обращаемся. Обычно они соответствуют названиям классов в программировании или коллекций в базе данных. К примеру, если там указано значение `users`, то эндпоинт `GET /api/v1/users`, вероятно, отвечает за _получение_ списка пользователей. Давай рассмотрим другой эндпоинт: `POST /api/v1/collection`. Скорее всего, он отвечает за добавление какой-то коллекции. 

В задании же требуется описать 4 эндпоинта с методами из CRUD (один эндпоинт на каждый метод). Тему приложения ты уже знаешь!

## Эндпоинты
Вот четыре эндпоинта для приложения, которое позволяет работать с рецептами новогодних блюд, используя все методы CRUD:

1. **GET /api/v1/recipes**: Получить список всех рецептов новогодних блюд.
2. **POST /api/v1/recipes**: Добавить новый рецепт новогоднего блюда.
3. **PUT /api/v1/recipes/{id}**: Обновить информацию о конкретном рецепте новогоднего блюда по его идентификатору.
4. **DELETE /api/v1/recipes/{id}**: Удалить рецепт новогоднего блюда по его идентификатору.

Здесь "v1" представляет собой версию API, а "recipes" является классом объектов, с которыми работает приложение.
