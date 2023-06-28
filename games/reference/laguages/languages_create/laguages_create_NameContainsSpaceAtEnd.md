### Games reference/languages/ 
###### POST reference_languages_create
###### language name contains a space at the beginning of the word

### *Step:*
1. Создать в Postman новый запрос: ***POST***, url: https://games.alpha.g-spot.website/api/v1/reference/languages/
2. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
         "name": "ru "
         }

3. Заполнить вкладку ***Authorization*** [данными для авторизации](https://github.com/victoretc/GSPOTtestingdocumentation/blob/main/Authorization_data.md)
4. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 201 - Created

body ( json, id назначается автоматически, может отличаться от скрина ниже ):

      { 
         "id": 1,  
         "name": "ru" 
      }


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------|-----------| --- | --- |
| 2023-06-26 | 12:05 | Passed    | IvanKorolev13 | --- | 
