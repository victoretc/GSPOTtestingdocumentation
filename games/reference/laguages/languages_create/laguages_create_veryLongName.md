### Games reference/languages/ 
###### POST reference_languages_create
###### language name is very long

### *Step:*
1. Создать в Postman новый запрос: ***POST***, url: https://games.alpha.g-spot.website/api/v1/reference/languages/
2. Заполнить вкладку ***body***: чек-бокс- ***row***, тип отображения- сменить Text на ***JSON***, в поле ввода ввести-

        {
         "name": "qwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopAasdfghjklzxcvbnmqwertyuiopasdfghjklzxcvbnmqwertyuiopasdfghjklzxcvbnmqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopAasdfghjklzxcvbnmqwertyuiopasdfghjklzxcvbnmqwertyuiopasdfghjklzxcvbnmqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopqwertyuiopAasdfghjklzxcvbnmqwertyuiopasdfghjklzxcvbnmqwertyuiopasdfghjklzxcvbnm"
         }

3. Заполнить вкладку ***Authorization***: type- ***Basic Auth***, Username- ***tester***, Password- ***tester***
4. Нажать "***Send***" ("Отправить")

### *Expected result:*
    Server response: status code 400 - Bad Request

body:

      {
         "name": [
            "Убедитесь, что это значение содержит не более 100 символов."
         ]
      }


Автор: IvanKorolev13

Тест done

| Дата       | Время | Результат | Имя | Баг № Trello |
|------------|-------| --- | --- | --- |
| 2023-07-06 | 17:05 | Passed | IvanKorolev13 | --- | 