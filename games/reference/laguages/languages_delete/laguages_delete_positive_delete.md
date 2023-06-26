### Games reference/languages/id/ 
###### DELETE reference_languages_delete

### *Pre-conditions:*
1. Отчистить данные из БД "Language"
2. Создать методом POST https://games.alpha.g-spot.website/api/v1/reference/languages/ запрос с body:


      {
         "name": "ru"
      }

3. Переписать id полученный в Response Body (теле ответа)

### *Step:*
1. Создать в Postman новый запрос: ***DELETE***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 204 - No content

4. Создать в Postman новый запрос: ***GET***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/***
5. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
6. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 200 - OK
body ( json ): отсутствует запись с "id": id, полученный в Pre-conditions

### *Post-conditions:*
1. Отчистить данные из БД "Language"


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-06-23 | 11:15 | Passed | IvanKorolev13 | --- | 