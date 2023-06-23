### Games reference/product_languages/id/ 
###### PUT reference_product_languages_update

### *Pre-conditions:*
1. Создать методом POST https://games.alpha.g-spot.website/api/v1/reference/product_languages/ два запроса с body:


      {
         "languageName":"RU",
         "interface": true,
         "subtitles": true,
         "voice": true
      }

2. Переписать id полученный в Response Body (теле ответа)

### *Step:*
1. Создать в Postman новый запрос: ***PUT***, url: ***https://games.alpha.g-spot.website/api/v1/reference/product_languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
            "languageName":"RUS",
            "interface": true,
            "subtitles": true,
            "voice": true
        }

4. Нажать "***Send***" ("Отправить")
5. Создать в Postman новый запрос: ***GET***, url: ***https://games.alpha.g-spot.website/api/v1/reference/product_languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
6. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
7. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 200 - OK

body ( json, "id": id, полученный в Pre-conditions ):

      { 
         "id": 1,  
         "languageName":"RUS",
         "interface": true,
         "subtitles": true,
         "voice": true 
      }

### *Post-conditions:*
1. Отчистить данные из БД "ProductLanguage"


Автор: IvanKorolev13

ест skipped

| Дата | Время | Результат | Имя | Баг № Trello |
|------|-------|-----------| --- | --- |
| ---  | ---   | skipped   | IvanKorolev13 | --- |