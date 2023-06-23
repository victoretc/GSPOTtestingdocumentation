### Games reference/languages/
###### GET reference_languages_list

### *Pre-conditions:*
1. Отчистить данные из БД "Language"
2. Создать методом POST https://games.alpha.g-spot.website/api/v1/reference/languages/ два запроса с body: 
   1. {"name": "ru"} 
   2. {"name": "en"}
   
### *Step:*
1. Создать в Postman новый запрос: ***GET***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/***
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 200 - OK

body ( json, id назначается автоматически, может отличаться от скрина ниже ):

    [
        { 
            "id": 1,  
            "name": "ru" 
        },
        { 
            "id": 2,  
            "name": "en" 
        } 
    ] 

### *Post-conditions:*
1. Отчистить данные из БД "Language"


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-06-22 | 23:10 | Passed | IvanKorolev13 | --- | 