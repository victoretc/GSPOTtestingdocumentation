### Payments
#### Payment Accounts Payment Commission (negative_fractional_number)

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/payment_commission/


1. Запустить Postman
2. Создать новый запрос
3. Выбрать метод POST
4. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/payment_commission/
5. Ввести в Body (json):
{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "payment_amount": -0,525
}
5. Отправить запрос

Ожидаемый результат: 	 Error: response status is 400
{
  "detail": "JSON parse error - Expecting ',' delimiter: line 4 column 23 (char 88)"
}


Автор: Георгий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-18 | 23:39 | Passed | Георгий | - | 