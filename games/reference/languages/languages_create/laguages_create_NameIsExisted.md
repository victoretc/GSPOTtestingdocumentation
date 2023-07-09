### Games reference/languages/ 
###### POST reference_languages_create
###### language name is existed

### *Step:*
1. Создать в Postman новый запрос: ***POST***, url: https://games.alpha.g-spot.website/api/v1/reference/languages/
2. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
         "name": "ru"
         }

3. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
4. Нажать "***Send***" ("Отправить")
5. Нажать еще раз "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 400 - Bad request

body:

      {
         "name": [
            "{сообщение об ошибке}"
         ]
      }


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------|-----------| --- | --- |
| 2023-06-24 | 17:50 | Failed    | IvanKorolev13 | --- | 