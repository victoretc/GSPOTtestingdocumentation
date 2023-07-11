### Payments
#### External Payments Payment Commission {id} (negative - non existent payment_service_id)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/{id}/


Предусловия:    1) сервис не должен быть создан 
                2) данные должны быть созданы (с помощью /v1/external_payments/commissions/ - метод POST)


1. Создать новый запрос в Postman
2. Выбрать метод PUT для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/30/
4. Ввести в Body -> raw -> JSON:
{
  "payment_type": "bank_card",
  "commission": "1",
  "payment_service_id": 107
}
5. Отправить Request

Ожидаемый результат: Server response: status code 400 - bad request

Body response:

{
    "payment_service_id": [
        "Invalid pk \"107\" - object does not exist."
    ]
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-11 | 15:15 | Passed | Евгений | - | 