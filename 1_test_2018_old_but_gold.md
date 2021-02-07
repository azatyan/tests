# Тест для соискателя на должность backend разработчика
Нужно реализовать REST API для базы данных роботов.

В REST API должны быть следующие вызовы

### Получение всех роботов

1. Url: http://example.com/api/robots
2. Method: GET

Пример запроса:
curl -i -X GET http://example.com/api/robots

### Поиск робота
1. Url: http://example.com/api/robots/search/:name
2. Method: GET
3. Data: {name: "Название робота"}

Пример
curl -i -X GET http://example.com/api/robots/search/Astro

### Получение робота по ID
1. Url: http://example.com/api/robots/:id
2. Method: GET
3. Data: {id: "ID робота"}

Пример
curl -i -X GET http://example.com/api/robots/3

### Добавление робота
1. Url: http://example.com/api/robots
2. Method: POST
3. Data: {"name":"Название робота","type":"Тип робота","year":Год создания}

Пример
curl -i -X POST -d '{"name":"C-3PO","type":"droid","year":1977}' http://example.com/api/robots

### Редактирование робота
1. Url: http://example.com/api/robots
2. Method: PUT
3. Data: {"id": "ID робота","name":"Название робота","type":"Тип робота","year":Год создания}

Пример
curl -i -X PUT -d '{"id": 1, "name":"ASIMO","type":"humanoid","year":2000}' http://example.com/api/robots/4

### Удаление робота
1. Url: http://example.com/api/robots/:id
2. Method: DELETE
3. Data: {id: "ID робота"}

Пример
curl -i -X DELETE http://example.com/api/robots/4

## Данный REST API нужно сделать используя фрэймворк SymfonyFlex и базу данных Mysql/MariaDB/Postgress

Результат работы должен оказаться в GIT репозитории

## Советы
1. Не забываем работать с репозиторием. Для git является хорошей практикой делать много коммитов(commit) и меньше пушей (push)
2. Не забываем комментировать код. Не нужно фанатизма, достаточно описание функций и сложных участков кода внутри функций.
3. Если вам кажется что потратили уже много времени, вполне можете выложить то что уже есть. Возможно этого будет достаточно.
4. Не делайте ТТУК (Толстые тупые уродливые контроллеры) - добавьте сервисный слой для бизнес логики

### Если возникнут трудности задавайте вопросы, по возможности будем помогать!

## Удачи вам в выполнении этого задания
