### Payments
#### External Payments Payment Commission (positive)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/{id}


Предусловия:    1)сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST) - из него берется id для "payment_service_id"
                2) данные должны быть созданы (с помощью /v1/external_payments/commissions/ - метод POST)


1. Создать новый запрос в Postman
2. Выбрать метод PATCH для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/7/
4. Ввести в Body -> raw -> JSON:

{
  "payment_type": "string",
  "commission": "5",
  "payment_service_id": 8
}

5. Отправить Request

Ожидаемый результат: Server response: status code 200 - OK

Body response:

{
    "id": 7,
    "payment_type": "string",
    "commission": "5.00",
    "payment_service_id": 8
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-30 | 12:30 | Passed | Евгений | - | 