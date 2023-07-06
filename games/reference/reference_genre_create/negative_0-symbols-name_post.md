POST negative 0 symbols name
===

Предварительные условия
--

1. [Информация по авторизации](https://github.com/victoretc/GSPOTtestingdocumentation/blob/main/games/Authorization_data.md).
2. Тестовые данные:

name = ""
id не меняем

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
{
  "name": "",
  "id": "<integer>"
}

4. Отправить запрос

Ожидаемый результат
--
1. Status ответа: 400 Bad Request.
2. В ответе вернулось:

```
{
    "name": [
        "Это поле не может быть пустым."
    ]
}
```

Автор: Анастасия

Прохождение тест-кейса:
----------------

|**Дата**|**Время**|**Результат**|**Имя**|**Баг № Trello**|
| :-: | :-: | :-: | :-: | :-: |
|27.06.2023|19:15|Passed|negative_0-symbols-name_post|-|