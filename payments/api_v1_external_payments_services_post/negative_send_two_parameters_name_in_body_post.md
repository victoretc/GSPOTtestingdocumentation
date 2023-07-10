### Payments
#### External_payments_services_negative_send_two_parameters_name_in_body_post

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/external_payments/services/


1. Создать новый запрос в Postman=>выбрать метод POST 
2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/external_payments/services/
3. Выбрать вкладку body=>тип raw=> формат JSON
4. Вставить данные в окно ввода:
{
  "name": "string"
}
5. Создать дубликат поля "name" с разными значениями 
6. Нажать кнопку “Send”


Ожидаемый результат: Server response status code 400 Bad Request 

Body response:
{
    "detail": "JSON parse error - Expecting ',' delimiter: line 3 column 3 (char 22)"
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя  | Баг № Trello|
|     ---    |  ---  |    ---    |   ---  |      ---    |
| 2023-07-06 | 13:05 |   Passed  | Василий|       -     | 