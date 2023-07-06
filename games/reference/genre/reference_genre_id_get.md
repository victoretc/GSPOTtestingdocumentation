### Games reference
#### Get genre id


1. Запустить Postman
2. Создать запрос
- метод - GET
- URL - games.alpha.g-spot.website/api/v1/reference/genre/
key = id, value = 1
3. Вкладка Authorization
Авторизоваться: использовать валидные значения Username:tester, Password:tester
5. Отправить запрос

Ожидаемый результат:
1. Status ответа: 200 OK.

2. В теле ответа вернулись id и название запрошенного жанра. Пример:

```
{
  "id": 1,
  "name": "string"
}

Автор: Ксения


| Дата | Время | Результат | Имя | Баг № Trello |
| ---  | ---   | ---       | --- | ---    |
| 2023-06-10 | 23:40 | FAILED | Ксения |https://trello.com/c/JOnS0Khc| 