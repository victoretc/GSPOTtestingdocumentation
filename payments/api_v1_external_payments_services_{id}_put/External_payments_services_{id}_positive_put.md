### Payments
#### External_payments_services_{id}_positive_put

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

Предусловия: сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST)

1. Создать новый запрос в Postman, выбрать метод PUT

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

4. Ввести в конец URL номер id существующего сервиса через / (/7/)

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "name": "string"
}

5. Ввести данные в поле "name"-"sber"

5. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 200 Ok

Body response:

[
  {
    "id": 7,
    "name": "sber"
  }
]


Автор: Василий

Тест выполнен
|     Дата      | Время | Результат |   Имя   | Баг № Trello |
|     ---       |  ---  |    ---    |   ---   |      ---     |
|  2023-06-28   | 13:31 |   Passed  | Василий |       -      | 