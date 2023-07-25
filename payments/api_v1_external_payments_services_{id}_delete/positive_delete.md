### Payments
#### External_payments_services_{id}_positive_delete

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

Предусловия: сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST)

1. Создать новый запрос в Postman, выбрать метод DELETE

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

3. Ввести в конец URL номер id существующего сервиса через / (/7/)

4. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 204 Ok

Body response: 	
No response body



Автор: Василий

Тест выполнен
|     Дата    | Время | Результат|   Имя  | Баг № Trello|
|     ---     |  ---  |    ---   |   ---  |      ---    |
|  2023-06-28 | 13:50 |   Passed | Василий|       -     | 