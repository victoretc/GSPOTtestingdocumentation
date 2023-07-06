Payments 
PAYOUT FOR DEVELOPERS 

Тестовые данные: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/

Создать новый запрос в Postman
Выбрать метод POST для Request
Ввести URL: https://payments.alpha.g-spot.website/v1/payments_accounts/payout/
Ввести в Body -> raw -> JSON: {"amount": {"value", "currency", "payout_destination_data": "type_", "account_number", "user_uuid"
Отправить Request
Ожидаемый результат: Server response: status code 200 - OK

Постусловие: удалить тестовые данные

Автор: Юлия

Постусловие: удалить тестовые данные

Дата	Время	Результат	Имя	Баг № Trello
2023-07-06	18:05	Passed	Юлия
