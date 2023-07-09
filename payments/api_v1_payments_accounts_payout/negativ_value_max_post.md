Payments

PAYOUT FOR DEVELOPERS

Тестовые данные: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/

1.Создать новый запрос в Postman

2.Выбрать метод POST для Request

3.Ввести URL: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/

4.Ввести в Body -> raw -> JSON: { "amount": { "value": 777777777777, "currency": "RUB" }, "payout_destination_data": { "type_": "BANK_CARD", "account_number": "RRRRRFF344" }, "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6" }

Отправить Request

Ожидаемый результат: Server response: 400 Bad Request

"amount": {
        "value": [
            "Ensure that there are no more than 11 digits in total."
            ]
    }
}


Автор: Юлия

Тест выполнен

09.07.2023
