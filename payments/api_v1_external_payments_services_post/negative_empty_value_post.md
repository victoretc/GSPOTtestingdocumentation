### Payments
#### External_payments_services_negative_empty_value_post

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/


1. Создать новый запрос в Postman=>выбрать метод POST 
2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/
3. Выбрать вкладку body=>тип raw=> формат JSON
4. Вставить данные в окно ввода:
{
  "name": "string"
}
5. Оставить пустым поле "name" (пример "")
6. Нажать кнопку “Send”


Ожидаемый результат: Server response status code 400 Bad Request 

Body response:
{
    "name": [
        "This field may not be blank."
    ]
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя  | Баг № Trello|
|     ---    |  ---  |    ---    |   ---  |      ---    |
| 2023-07-01 | 20:28 |   Passed  | Василий|       -     | 