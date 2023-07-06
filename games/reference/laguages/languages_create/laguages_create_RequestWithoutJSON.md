### Games reference/languages/ 
###### POST reference_languages_create
###### request is without Json

### *Step:*
1. Создать в Postman новый запрос: ***POST***, url: https://games.alpha.g-spot.website/api/v1/reference/languages/
2. НЕ Заполнить вкладку ***body***
3. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
4. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 400 - Bad Request

body:

      {
         "name": [
            "Обязательное поле."
            ]
      }


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-07-06 | 17:05 | Passed | IvanKorolev13 | --- | 