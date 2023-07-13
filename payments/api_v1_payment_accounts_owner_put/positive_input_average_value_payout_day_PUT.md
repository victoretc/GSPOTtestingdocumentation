### Payments
#### Payment_accounts_owner_positive_input_average_value_payout_day_PUT

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

5. Ввести среднее значение в поле "payout_day_of_month"-(пример 13)

6. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 200 ok

Body response:
{
    "id": 1,
    "revenue_currency": "RUB",
    "revenue": "0.00",
    "income_currency": "RUB",
    "income": "0.00",
    "commission": "100.00",
    "frozen_time": "00:00:00",
    "gift_time": "00:00:00",
    "payout_day_of_month": 13
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-13 | 16:24 |   Passed  | Василий|     -      | 