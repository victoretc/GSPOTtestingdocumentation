### Games utils filters
#### GET prices

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/utils/filters/prices?limit=5&offset=10

**Type:** API

**Preconditions**:
1. Запустить Postman

**STR**
1. Создать новый запрос
2. Выбрать метод GET для Request
5. Ввести URL: https://games.alpha.g-spot.website/api/v1/utils/filters/prices?limit=5&offset=10
6. Нажать Send

**Expected Result:**
Server response: status code 200 - OK
```json 
{
  "count": 0,
  "next": "string",
  "previous": "string",
  "results": [
    {
      "minPrice": "string",
      "maxPrice": "string"
    }
  ]
}
```

Автор: Вячеслав

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-15 | 17:00 | PASSED | Вячеслав | | 
