### Payments
#### Transactions_purchase_positive

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/transactions/purchase/


1. Создать новый запрос в Postman, выбрать метод POST

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/transactions/purchase/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода                                                                           {"payment_type": "bank_card","payment_service": "yookassa","user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6","items_payment_data": [{"owner_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6","item_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6","developer_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6","price": 999999999}],"return_url": "string"}

5. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 201 Ok

Body response:

{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "items_payment_data": [
    {
      "owner_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
      "item_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
      "developer_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
      "price": 999999999
    }
  ],
  "return_url": "string"
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата   | Время | Результат |   Имя   | Баг № Trello |
|     ---    |  ---  |    ---    |   ---   |      ---     |
| 2023-06-16 | 16:20 |   Failed  | Василий | https://trello.com/c/oHCMCntQ/214-400-bad-request-transactionspurchasepositive-%D0%BD%D0%B0-%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-post | 