POST positive digits name
===

Предварительные условия
--

1. [Информация по авторизации](https://github.com/victoretc/GSPOTtestingdocumentation/blob/main/games/Authorization_data.md).

2. Тестовые данные:
name = "0123456789"

id - не меняем.

Действия в Postman
--
1. Создать запрос
- метод - POST
- URL - games.alpha.g-spot.website/api/v1/reference/genre/

2. Вкладка Authorization
ввести данные по авторизации - см. информацию по авторизации в предварительных условиях.

3. Вкладка Body
- выбрать тип raw
- выбрать формат JSON
- тело запроса:

```json
{
  "name": "0123456789",
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
    "id": 109,
    "name": "0123456789"
}
```

Автор: Анастасия

Прохождение тест-кейса:
----------------

|**Дата**|**Время**|**Результат**|**Имя**|**Баг № Trello**|
| :-: | :-: | :-: | :-: | :-: |
|27.06.2023|19:15|Passed|positive_digits-name_post|-|
