### Payments
#### Payment_accounts_owner_negative_empty_value_payout_day_PUT

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PUT

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "100",
  "frozen_time": "00:00:00",
  "gift_time": "00:00:00",
  "payout_day_of_month": 13
}

5. Удалить значение в поле "payout_day_of_month"

6. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 400 Bad Request
Body response:
{
    "detail": "JSON parse error - Expecting value: line 6 column 1 (char 111)"
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-13 | 16:34 |   Passed  | Василий|     -      | 