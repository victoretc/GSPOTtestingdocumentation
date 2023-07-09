### Payments
#### External_payments_services_negative_send_empty_body_post

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/


1. Создать новый запрос в Postman=>выбрать метод POST 
2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/
3. Выбрать вкладку body=>тип raw=> формат JSON
4. Оставить поле ввода параметров body пустым
6. Нажать кнопку “Send”


Ожидаемый результат: Server response status code 400 Bad Request 

Body response:
{
    "name": [
        "This field is required."
    ]
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя  | Баг № Trello|
|     ---    |  ---  |    ---    |   ---  |      ---    |
| 2023-07-06 | 13:15 |   Passed  | Василий|       -     | 