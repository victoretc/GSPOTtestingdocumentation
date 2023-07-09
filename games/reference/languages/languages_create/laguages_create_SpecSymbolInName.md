### Games reference/languages/ 
###### POST reference_languages_create
###### language name is with spec symbol

### *Step:*
1. Создать в Postman новый запрос: ***POST***, url: https://games.alpha.g-spot.website/api/v1/reference/languages/
2. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
         "name": "~!@#$%^&*()_+<>?:\"|{}[]';,.`-="
         }

3. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
4. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 400 - Bad Request

body:

      {
         "name": [
            "{сообщение об ошибке}"
         ]
      }


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello                                                                                           |
|------------|-------|-----------| --- |--------------------------------------------------------------------------------------------------------|
| 2023-06-24 | 16:05 | Failed    | IvanKorolev13 | [Bug Report](https://trello.com/c/xP5eKVPn/232-the-language-name-is-created-from-only-special-symbols) | 