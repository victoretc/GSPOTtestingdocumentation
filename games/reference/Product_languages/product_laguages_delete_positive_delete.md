### Games reference/product_languages/id/ 
###### DELETE reference_product_languages_delete

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
1. Создать в Postman новый запрос: ***DELETE***, url: ***https://games.alpha.g-spot.website/api/v1/reference/product_languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 204 - No content

4. Создать в Postman новый запрос: ***GET***, url: ***https://games.alpha.g-spot.website/api/v1/reference/product_languages/***
5. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
6. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 200 - OK
body ( json ): отсутствует запись с "id": id, полученный в Pre-conditions

### *Post-conditions:*
1. Отчистить данные из БД "ProductLanguage"


Автор: IvanKorolev13

ест skipped

| Дата | Время | Результат | Имя | Баг № Trello |
|------|-------|-----------| --- | --- |
| ---  | ---   | skipped   | IvanKorolev13 | --- |