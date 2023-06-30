### Payments
#### Payment Accounts Payment Commission (negative - negative amount)

Тестовые данные: https://payments.alpha.g-spot.website/v1/payment_accounts/payment_commission/


1. Создать новый запрос в Postman
2. Выбрать метод POST для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/payment_accounts/payment_commission/
4. Ввести в Body -> raw -> JSON:
{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "payment_amount": -1
}
5. Отправить Request

Ожидаемый результат: Server response: status code 400 - Bad Request
{
    "payment_amount": [
        "Insufficient Funds"
    ]
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-14 | 11:05 | Passed | Евгений | - | 