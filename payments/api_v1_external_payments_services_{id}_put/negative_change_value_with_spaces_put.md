### Payments
#### External_payments_services_{id}_negative_change_value_with_spaces_put

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

Предусловия: сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST)

1. Создать новый запрос в Postman, выбрать метод PUT

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/

4. Ввести в конец URL номер id существующего сервиса через / (пример /25/)

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "name": "string"
}

5. Ввести пробелы в поле "name"-(пример "     ")

5. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 400 Bad Request

Body response:
{
    "name": [
        "This field may not be blank."
    ]
}


Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя  | Баг № Trello|
|     ---    |  ---  |    ---    |   ---  |    ---      |
|  2023-07-06| 13:31 |   Passed  |Василий |      -      | 