### Games reference/languages/ 
###### GET reference_languages_list

### *Pre-conditions:*
1. Отчистить данные из БД "Language"
2. Создать методом POST https://games.alpha.g-spot.website/api/v1/reference/languages/ два запроса с body:

   
      I.
      {
         "name": "ru"
      }

      II.
      {
         "name": "en"
      }
   
### *Step:*
1. Создать в Postman новый запрос: ***GET***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/***
2. Установить во вкладке Params два параметра: 
     Key- limit, Value- 1, 
     Key- offset, Value-  {пустое значение}
3. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
4. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 200 - OK

body ( json, id назначается автоматически, может отличаться от скрина ниже ):

    {
          "count": 2,
          "next": "https://games.alpha.g-spot.website/api/v1/reference/languages/?limit=1&offset=1",
          "previous": null,
          "results": [
               {
                    "id": 1,
                    "name": "ru"
               }
          ]
     }

### *Post-conditions:*
1. Отчистить данные из БД "Language"


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-07-06 | 17:45 | Passed | IvanKorolev13 | --- | 