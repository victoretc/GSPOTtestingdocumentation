Payments 

PAYOUT FOR DEVELOPERS 

Тестовые данные: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/

1.Создать новый запрос в Postman

2.Выбрать метод POST для Request

3.Ввести URL: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/

4.Ввести в Body -> raw -> JSON: {
  "amount": {
    "value": 500,
    "currency": "USD"
  },
  "payout_destination_data": {
    "type_": "Paypal",
    "account_number": "string"
  },
  "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
}

Отправить Request

Ожидаемый результат: Server response: 400 Bad Request

{
    "payout_destination_data": {
        "type_": [
            "\"Paypal\" is not a valid choice."
        ]
    }
}
Автор: Юлия

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-09 | 15:40 | Passed | Юлия | - | 
