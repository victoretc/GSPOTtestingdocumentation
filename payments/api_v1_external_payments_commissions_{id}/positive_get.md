### Payments
#### External Payments Payment Commission {id} (positive)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/{id}

Предусловие: данные должны быть созданы (с помощью /v1/external_payments/commissions/ - метод POST)

1. Создать новый запрос в Postman
2. Выбрать метод GET для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/7/
4. Отправить Request

Ожидаемый результат: Server response: status code 200 - OK

Body response:

{
    "id": 7,
    "payment_type": "string",
    "commission": "1.00",
    "payment_service_id": 8
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-30 | 12:00 | Passed | Евгений | - | 