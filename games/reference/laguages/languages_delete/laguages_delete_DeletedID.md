### Games reference/languages/id/ 
###### DELETE reference_languages_delete
###### id is not existed

### *Pre-conditions:*
1. Отчистить данные из БД "Language"
2. Создать методом GET https://games.alpha.g-spot.website/api/v1/reference/languages/ список существующих записей
3. Выбрать id, которого существует в полученном списке
4. Удалить данный id методом DELETE

### *Step:*
1. Создать в Postman новый запрос: ***DELETE***, url: ***https://games.alpha.g-spot.website/api/v1/reference/languages/0/*** (**вместо 0 вставить id полученный в Pre-conditions**)
2. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
3. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 404 - Not Found

body:

        {
            "detail": "Страница не найдена."
        }



Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-07-06 | 17:35 | Passed | IvanKorolev13 | --- | 