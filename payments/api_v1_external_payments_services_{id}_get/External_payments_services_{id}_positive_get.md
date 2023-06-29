### Payments
#### External_payments_services_{id}_positive_get

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

Предусловия: сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST)

1. Создать новый запрос в Postman, выбрать метод POST

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

3. Ввести в конец URL номер id существующего сервиса через / (/7/)

4. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 200 Ok

Body response:

{
  "id": 7,
  "name": "qiwi"
}



Автор: Василий

Тест выполнен
|     Дата      | Время | Результат |   Имя   | Баг № Trello |
|     ---       |  ---  |    ---    |   ---   |      ---     |
|  2023-06-28   | 13:24 |   Passed  | Василий |       -      | 