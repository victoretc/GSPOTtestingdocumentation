### Games reference/languages/id/
###### PATCH reference_languages_partial_update

### *Pre-conditions:*
1. Отчистить данные из БД "Language"
2. Создать методом POST https://games.alpha.g-spot.website/api/v1/reference/languages/ два запроса с body:


      {
         "name": "ru"
      }

3. Переписать id полученный в Response Body (теле ответа)

### *Step:*
1. Создать в Postman новый запрос: ***PATCH***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
         "name": "RUS"
         }

4. Нажать "***Send***" ("Отправить")
5. Создать в Postman новый запрос: ***GET***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
6. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
7. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 200 - OK

body ( json, "id": id, полученный в Pre-conditions ):

      { 
         "id": 1,  
         "name": "RUS" 
      }

### *Post-conditions:*
1. Отчистить данные из БД "Language"


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-06-23 | 11:15 | Passed | IvanKorolev13 | --- |** 