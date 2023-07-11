### Payments
#### External Payments Payment Commission (positive)

Тестовые данные: https://payments.alpha.g-spot.website/v1/external_payments/commissions/

Предусловие: данные должны быть созданы (с помощью /v1/external_payments/commissions/ - метод POST)

1. Создать новый запрос в Postman
2. Выбрать метод GET для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/external_payments/commissions/
4. Отправить Request

Ожидаемый результат: Server response: status code 200 - OK

Body response:

[ 
    { "id": 5, 
    "payment_type": "bank_card", 
    "commission": "10.58", "payment_service_id": 8 
    }, 
    { "id": 6, 
    "payment_type": "string", 
    "commission": "10.00", "payment_service_id": 8 
    }, 
    { "id": 7, 
    "payment_type": "string", 
    "commission": "1.00", 
    "payment_service_id": 8 
    } 
]


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-30 | 10:40 | Passed | Евгений | - | 