### Payments
#### External_payments_services_{id}_negative_remove_multiple_services_delete

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/


1. Создать новый запрос в Postman, выбрать метод DELETE

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

3. Ввести в конец URL номера id несуществующих сервисов через , (пример /1, 2/); либо через / (пример /1/2/)

4. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 404 Not Found

Body response: 	
{
    "detail": "Not found."
}



Автор: Василий

Тест выполнен
|     Дата    | Время | Результат|   Имя  | Баг № Trello|
|     ---     |  ---  |    ---   |   ---  |      ---    |
|  2023-07-07 | 13:57 |   Passed | Василий|       -     | 