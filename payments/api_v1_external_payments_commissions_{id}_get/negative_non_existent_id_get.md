### Payments
#### External Payments Payment Commission {id} (negative - non-existent id)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/{id}

Предусловие: данные должны быть созданы (с помощью /v1/external_payments/commissions/ - метод POST)

1. Создать новый запрос в Postman
2. Выбрать метод GET для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/105/
4. Отправить Request

Ожидаемый результат: Server response: status code 404 - not found

Body response:

{
    "detail": "Not found."
}

Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-06 | 15:30 | Passed | Евгений | - | 