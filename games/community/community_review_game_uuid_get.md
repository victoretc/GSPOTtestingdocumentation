### Games community
#### Get comments

Тестовые данные: https://games.alpha.g-spot.website/api/v1/community/review/3/?limit=10&offset=5

1. Запустить Postman
2. Создать новую коллекцию или импортировать информацию с swaggera https://games.alpha.g-spot.website/swagger/?format=openapi
3. Создать новый запрос
4. Авторизироваться: используя валидные значения Username:tester, Password:tester(в Postman выбрать пункт Autorization)
5. Выбрать метод GET для Request
6. Ввести URL: https://games.alpha.g-spot.website/api/v1/community/review/3/?limit=10&offset=5
7. Отправить Request

Ожидаемый результат:
Server response: status code 200 - OK
{
  "count": 0,
  "next": "string",
  "previous": "string",
  "results": [
    {
      "id": 0,
      "reactions": "string",
      "language": "string",
      "userUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
      "text": "string",
      "grade": "LIKE",
      "viewType": true,
      "canReply": true,
      "createdAt": "2023-06-12T06:34:19.872Z"
    }
  ]
}
Постусловие: удалить тестовые данные

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-10 | 12:35 | FAIL | Дмитрий | https://trello.com/c/Ycxrefru | 