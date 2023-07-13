Payments

PAYOUT DATA

Тестовые данные: https://payments.alpha.g-spot.website/v1/payments_accounts/payout_data/

1.Создать новый запрос в Postman

2.Выбрать метод POST для Request

3.Ввести URL: https://payments.alpha.g-spot.website/v1/payments_accounts/payout_data/

4.Ввести в Body -> raw -> JSON: 

{
  "account_number": "11111",
  "is_auto_payout": true,
  "payout_type": "paypal",
  "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
}
Отправить Request

Ожидаемый результат: 400 Bad Request

{
    "payout_type": [
        "\"paypal\" is not a valid choice."
    ]
}

Автор: Юлия

Тест выполнен

13.07.2023
