### Games utils filters
#### Get genres

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/utils/filters/genres?limit=5&offset=10

**Type:** API

**Preconditions**:
1. Запустить Postman

 **STR**
1. Создать новый запрос
2. Выбрать метод GET для Request
3. Ввести URL: https://games.alpha.g-spot.website/api/v1/utils/filters/genres?limit=5&offset=10
4. Нажать "Send"

**Expected Result:**
Server response: status code 200 - OK
```json 
{
  "count": 0,
  "next": "string",
  "previous": "string",
  "results": [
    {
      "id": 0,
      "name": "string",
      "subgenres": [
        {
          "id": 0,
          "name": "string"
        }
      ]
    }
  ]
}
```

Автор: Вячеслав

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-15 | 16:50 | PASSED | Вячеслав | | 
