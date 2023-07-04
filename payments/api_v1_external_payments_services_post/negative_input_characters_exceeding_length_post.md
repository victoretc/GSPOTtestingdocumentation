### Payments
#### External_payments_services_negative_input_characters_exceeding_length_post

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/


1. Создать новый запрос в Postman=>выбрать метод POST 
2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/
3. Выбрать вкладку body=>тип raw=> формат JSON
4. Вставить данные в окно ввода:
{
  "name": "string"
}
5. Ввести символы превышающие длинну допустимых значений в поле "name" (более 30 символов пример "fhjthgld3845unfjlcns30567fgcjk")
6. Нажать кнопку “Send”


Ожидаемый результат: Server response status code 400 Bad Request 

Body response:
{
    "name": [
        "Ensure this field has no more than 30 characters."
    ]
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя  | Баг № Trello|
|     ---    |  ---  |    ---    |   ---  |      ---    |
| 2023-07-01 | 19:59 |   Passed  | Василий|       -     | 