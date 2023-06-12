### Games community
#### Get comments

Тестовые данные: https://games.alpha.g-spot.website/api/v1/core/product/

1. Запустить Postman
2. Создать новую коллекцию или импортировать информацию с swaggera https://games.alpha.g-spot.website/swagger/?format=openapi
3. Создать новый запрос
4. Авторизироваться: используя валидные значения Username:tester, Password:tester(в Postman выбрать пункт Autorization)
5. Выбрать метод POST для Request
6. Ввести URL: https://games.alpha.g-spot.website/api/v1/core/product/
7. Отправить Request

Ожидаемый результат:
Server response: status code 200 - OK
{
  "count": 0,
  "next": "string",
  "previous": "string",
  "results": [
    {
      "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
      "name": "string",
      "releaseDate": "2023-06-12",
      "genres": [
        "string"
      ],
      "systemRequirements": [
        {
          "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
          "operatingSystem": "LINUX"
        }
      ],
      "price": "string",
      "discount": 0,
      "isBought": false,
      "isFavorite": false
    }
  ]
}
Постусловие: удалить тестовые данные

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-10 | 13:48 | FAIL | Дмитрий | https://trello.com/c/3dzXq71d | 