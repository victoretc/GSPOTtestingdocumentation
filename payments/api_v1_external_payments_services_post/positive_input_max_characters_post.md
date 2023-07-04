### Payments
#### External_payments_services_positive_input_max_characters_post

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/


1. Создать новый запрос в Postman=>выбрать метод POST 
2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/
3. Выбрать вкладку body=>тип raw=> формат JSON
4. Вставить данные в окно ввода:
{
  "name": "string"
}
5. Ввести 30 символов в поле "name" (пример "fhjthgld3845unfjlcns30567fgcjk")
6. Нажать кнопку “Send”


Ожидаемый результат: Server response status code 201 Created Ok 

Body response:
{
    "id": 13,
    "name": "fhjthgld3845unfjlcns30567fgcjk"
}

Постусловие: удалить тестовые данные

Автор: Василий


Тест выполнен
|     Дата  | Время | Результат |   Имя   | Баг № Trello|
|     ---   |  ---  |    ---    |   ---   |      ---    |
| 2023-07-01| 19:53 |   Passed  | Василий |      -      | 