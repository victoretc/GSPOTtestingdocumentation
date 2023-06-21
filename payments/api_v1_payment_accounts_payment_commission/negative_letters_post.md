### Payments
#### Payment Commission (negative - letters in total)

Тестовые данные: https://payments.alpha.g-spot.website/v1/payment_accounts/payment_commission/


1. Создать новый запрос в Postman
2. Выбрать метод POST для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/payment_accounts/payment_commission/
4. Ввести в Body:
{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "payment_amount": money
}
5. Отправить Request

Ожидаемый результат: Server response: status code 400 - Bad Request
{
    "detail": "JSON parse error - Expecting value: line 4 column 21 (char 89)"
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-14 | 11:15 | Passed | Евгений | - | 