### Payments
#### Payment_accounts_owner_positive_GET

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman=>выбрать метод GET 
2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/
3. Нажать кнопку “Send”


Ожидаемый результат: Server response status code 200 Ok

Body response:
{
    "id": 1,
    "revenue_currency": "RUB",
    "revenue": "0.00",
    "income_currency": "RUB",
    "income": "0.00",
    "commission": "90.00",
    "frozen_time": "00:00:00",
    "gift_time": "00:00:00",
    "payout_day_of_month": 13
}


Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя  | Баг № Trello|
|     ---    |  ---  |    ---    |   ---  |      ---    |
| 2023-07-13 | 15:35 |   Passed  | Василий|       -     | 