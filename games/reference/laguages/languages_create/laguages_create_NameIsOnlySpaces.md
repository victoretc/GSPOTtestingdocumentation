### Games reference/languages/ 
###### POST reference_languages_create
###### language's name is only spaces

### *Step:*
1. Создать в Postman новый запрос: ***POST***, url: https://games.alpha.g-spot.website/api/v1/reference/languages/
2. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
         "name": "  "
         }

3. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
4. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 400 - Bad Request

body:

      {
         "name": [
            "Это поле не может быть пустым."
         ]
      }


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------|-----------| --- | --- |
| 2023-06-24 | 16:05 | Passed    | IvanKorolev13 | --- | 