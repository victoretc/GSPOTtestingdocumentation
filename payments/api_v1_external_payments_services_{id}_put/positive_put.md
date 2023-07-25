### Payments
#### External_payments_services_{id}_positive_put

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

Предусловия: сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST)

1. Создать новый запрос в Postman, выбрать метод PUT

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

3. Ввести в конец URL номер id существующего сервиса через / (/12/)

4. Выбрать вкладку body=>тип raw=> формат JSON

5. Вставить данные в окно ввода
{
  "name": "string"
}

6. Ввести данные в поле "name"-(пример "123")

7. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 200 ok

Body response:

{
    "id": 12,
    "name": "123"
}


Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-06 | 13:21 |   Passed  | Василий|     -      | 