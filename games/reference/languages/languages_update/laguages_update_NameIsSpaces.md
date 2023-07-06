### Games reference/languages/id/ 
###### PUT reference_languages_update

### *Pre-conditions:*
1. Отчистить данные из БД "Language"
2. Создать методом POST https://games.alpha.g-spot.website/api/v1/reference/languages/ два запроса с body:


      {
         "name": "ru"
      }

3. Переписать id полученный в Response Body (теле ответа)

### *Step:*
1. Создать в Postman новый запрос: ***PUT***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
         "name": "  "
         }

4. Нажать "***Send***" ("Отправить")


### *Expected result:*
    Server response: status code 400 - Bad request

body:

      {
         "name": [
            "Это поле не может быть пустым."
         ]
      }

### *Post-conditions:*
1. Отчистить данные из БД "Language"


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-06-23 | 11:05 | Passed | IvanKorolev13 | --- | 