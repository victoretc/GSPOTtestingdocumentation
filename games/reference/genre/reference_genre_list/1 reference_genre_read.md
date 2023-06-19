GET - 1 - reference genre read
===

Предварительные условия
--

1. [Информация по авторизации](https://github.com/nastyaist/GSPOTtestingdocumentation/blob/main/games/Authorization%20data.md).

2. Тестовые данные:

name = "puzzle"

id - не меняем.

Действия в Postman
--
1. Создать жанр по [тест-кейсу](ссылка) с тестовыми данными:
-  
- 

2. Создать запрос

- метод - GET

- URL - games.alpha.g-spot.website/api/v1/reference/genre/:id/

2. Вкладка Authorization

ввести данные по авторизации - см. информацию по авторизации в предварительных условиях.

3. Вкладка Params / таблица Path Variables
 
- для Key задать Value = 1 

- тело запроса:

```json
{
  "name": "puzzle",
  "id": "<integer>"
}
```

4. Отправить запрос

Ожидаемый результат
--

1. Status ответа: 201 Created.

2. В Body ответа вернулись id и name созданного жанра. Пример:

```
{
    "id": 33,
    "name": "new_genre"
}
```

Автор: Анастасия

Прохождение тест-кейса:
----------------

|**Дата**|**Время**|**Результат**|**Имя**|**Баг № Trello**|
| :-: | :-: | :-: | :-: | :-: |
||||||
