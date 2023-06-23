### Games reference/product_languages/id/ 
###### GET reference_product_languages_read

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
1. Создать в Postman новый запрос: ***GET***, url: ***https://games.alpha.g-spot.website/api/v1/reference/product_languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 200 - OK

body ( json, id назначается автоматически, может отличаться от скрина ниже ):

      { 
         "id": 1,  
         "languageName":"RU",
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