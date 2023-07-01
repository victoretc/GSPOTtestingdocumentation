### Payments
#### External_payments_services_negative_create_duplicate_name_post

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/


1. Создать новый запрос в Postman=>выбрать метод POST 
2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/
3. Выбрать вкладку body=>тип raw=> формат JSON
4. Вставить данные в окно ввода:
{
  "name": "string"
}
5. Ввести существующее имя в поле "name" (пример "card")
6. Нажать кнопку “Send”


Ожидаемый результат: Server response status code 400 Bad Request 

Body response:
{
    "name": [
        "payment service with this name already exists."
    ]
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя  | Баг № Trello|
|     ---    |  ---  |    ---    |   ---  |      ---    |
| 2023-07-01 | 20:05 |   Passed  | Василий|       -     | 