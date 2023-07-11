### Payments
#### External Payments Payment Commission (positive - space before commission)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/


Предусловия: сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST) - из него берется id для "payment_service_id"


1. Создать новый запрос в Postman
2. Выбрать метод POST для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/
4. Ввести в Body -> raw -> JSON:
{
  "payment_type": "bank_card ",
  "commission": " 1",
  "payment_service_id": 8
}
5. Отправить Request

Ожидаемый результат: Server response: status code 201 - OK

Body response:

{
    "id": 66,
    "payment_type": "bank_card",
    "commission": "1.00",
    "payment_service_id": 8
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-11 | 16:20 | Passed | Евгений | - | 