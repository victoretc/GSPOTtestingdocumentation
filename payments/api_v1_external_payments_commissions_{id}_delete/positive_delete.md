### Payments
#### External Payments Payment Commission {id} (positive)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/{id}

Предусловие: данные должны быть созданы (с помощью /v1/external_payments/commissions/ - метод POST)

1. Создать новый запрос в Postman
2. Выбрать метод DELETE для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/7/
4. Отправить Request

Ожидаемый результат: Server response: status code 204 - No Content

Body response:

No response body


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-30 | 12:40 | Passed | Евгений | - | 