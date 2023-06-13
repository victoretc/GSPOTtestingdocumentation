### Payments
#### Increase Balance

Тестовые данные: https://payments.alpha.g-spot.website/v1/payment_accounts/increase_balance/


1. Создать новый запрос в Postman
2. Выбрать метод POST для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/payment_accounts/increase_balance/
4. Ввести в Body:
{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "payment_amount": 999999999,
  "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "return_url": "string"
}
5. Отправить Request

Ожидаемый результат: Server response: status code 201 - OK
{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "payment_amount": 999999999,
  "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "return_url": "string"
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-13 | 21:00 | Failed | Евгений | https://trello.com/c/5JhiBEV8 | 