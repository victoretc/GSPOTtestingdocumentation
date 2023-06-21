### Games community
#### PUT comments

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/core/product/691c8f43-0698-4cde-842d-eb426193c80f/

**Type:** API

**Preconditions**: 
[Авторизоваться][a].

[a]: https://github.com/1fvwka/GSPOTtestingdocumentation/blob/main/Autorization.md

 **STR**

**1.Создать** новый запрос

**2.Выбрать** метод PUT для Request

**3.Ввести URL:** https://games.alpha.g-spot.website/api/v1/core/product/691c8f43-0698-4cde-842d-eb426193c80f/

**4.Выбрать вкладку** Body=>Raw=>JSON

**5.Ввести данные** в окно ввода Body 
```json 
{
  "name": "Велосипеды",
  "description": "string",
  "developersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "publishersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "langs": [
    {
      "languageName": "Russian",
      "interface": true,
      "subtitles": true,
      "voice": true
    }
  ]
}
 ```
 **6.Нажать  "Send"**

 **Expected Result:**
 Server response: status code: 200 - OK
```json
{
  "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "name": "Велосипеды",
  "description": "string",
  "developersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "publishersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "langs": [
    {
      "id": 0,
      "languageName": "Russian",
      "interface": true,
      "subtitles": true,
      "voice": true
    }
  ]
}

```
**Post conditions:** вернуть систему в первоначальное состояние

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-21 | 11:53 | FAIL | Дмитрий | https://trello.com/c/H7jIFdTi | 