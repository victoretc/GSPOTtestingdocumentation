POST negativespecify non-existing id
===

Предварительные условия
--

1. [Информация по авторизации](https://github.com/victoretc/GSPOTtestingdocumentation/blob/main/games/Authorization_data.md).
2. 14 > id последнего в списке жанра в БД > 14, но не равен 14.
3. Тестовые данные:

name = "инди"

id = "15"

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
  "name": "инди",
  "id": "15"
}
```

4. Отправить запрос

Ожидаемый результат
--

1. Status ответа: 201 Created.
2. В Body ответа вернулись id и name созданного жанра. id создан новый, не равен "15". Пример:

```
{
    "id": 111,
    "name": "инди"
}
```

Автор: Анастасия

Прохождение тест-кейса:
----------------

|**Дата**|**Время**|**Результат**|**Имя**|**Баг № Trello**|
| :-: | :-: | :-: | :-: | :-: |
|27.06.2023|19:15|Passed|negative_specify-non-existing-id-post|-|