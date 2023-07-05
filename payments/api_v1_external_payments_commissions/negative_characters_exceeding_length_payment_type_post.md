### Payments
#### External Payments Payment Commission (negative - characters exceeding lenght payment_type)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/


Предусловия: сервис должен быть создан (с помощью api/v1/external_payments/services/ метод POST) - из него берется id для "payment_service_id"


1. Создать новый запрос в Postman
2. Выбрать метод POST для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/
4. Ввести в Body -> raw -> JSON:
{
  "payment_type": "asdfghjkloiuytrvbknhjuyghbvfghjkjhgfdsaqwerfcdfvbgf", <!--51 символ>
  "commission": "1",
  "payment_service_id": 8
}
5. Отправить Request

Ожидаемый результат: Server response: status code 400 - bad request

Body response:

{
    "payment_type": [
        "Ensure this field has no more than 50 characters."
    ]
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-04 | 17:30 | Passed | Евгений | - | 