### Games reference/product_languages/ 
###### POST reference_product_languages_create

### *Step:*
1. Создать в Postman новый запрос: ***POST***, url: https://games.alpha.g-spot.website/api/v1/reference/product_languages/
2. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
            "languageName":"RU",
            "interface": true,
            "subtitles": true,
            "voice": true
         }

3. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
4. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 201 - Created

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

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello                                                                                                                                          |
|------------|-------|-----------| --- |-------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2023-06-23 | 14:33 | Failed    | IvanKorolev13 | [Bug-report](https://trello.com/c/CF7sIBCv/198-500-internal-server-error-%D0%BD%D0%B0-%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-post-reference-productlanguages) | 