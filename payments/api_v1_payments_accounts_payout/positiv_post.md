Payments 

PAYOUT FOR DEVELOPERS 

Тестовые данные: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/

1.Создать новый запрос в Postman
2.Выбрать метод POST для Request
3.Ввести URL: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/
4.Ввести в Body -> raw -> JSON: {"amount": {"value", "currency", "payout_destination_data": "type_", "account_number", "user_uuid"

Отправить Request

Ожидаемый результат: Server response: status code 200 - OK

{
  "amount": {
    "value": 500000,
    "currency": "RUB"
  },
  "payout_destination_data": {
    "type_": "BANK_CARD",
    "account_number": "string"
  },
  "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
}

Постусловие: удалить тестовые данные
Автор: Юлия

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-06 | 16:00 | Passed | Юлия | - | 

