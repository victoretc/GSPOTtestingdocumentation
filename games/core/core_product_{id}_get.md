### Games community
#### GET comments

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/core/product/691c8f43-0698-4cde-842d-eb426193c80f/

**Type:** API

**Preconditions**: 
[Авторизоваться][a].

[a]: https://github.com/1fvwka/GSPOTtestingdocumentation/blob/main/Autorization.md

 **STR**

**1.Создать** новый запрос

**2.Выбрать метод** GET для Request

**3.Ввести URL** https://games.alpha.g-spot.website/api/v1/core/product/691c8f43-0698-4cde-842d-eb426193c80f/

**4.Нажать:** "Send"

 **Expected Result:**
 Server response: status code: 200 - OK
```json
{
  "id": "691c8f43-0698-4cde-842d-eb426193c80f",
  "name": "Cyclemania",
  "releaseDate": "2023-06-19",
  "genres": [],
  "price": 1,
  "discount": 0,
  "isBought": false,
  "isFavorite": false,
  "description": "In Cyclemania you’ll push your motorcycle and your skills to the limit on five uniquely difficult courses – all created directly from video of real roads. Using impressive video compression and variable frame-rate decompression techniques, Cyclemania lets you race along twisting, turning mountain roads at speeds of over 150 miles per hour.",
  "about": "Непонятно, зачем нужно это поле. Какое-то ещё описание.",
  "age": 18,
  "adult": "true",
  "status": "MODERATION",
  "type": "GAMES",
  "developersUuid": "803548a7-3334-435a-995a-be8dfc056399",
  "publishersUuid": "857d2d74-8e36-4fa3-bd2d-73330332192b",
  "dlcs": [],
  "langs": [
    {
      "id": 2,
      "languageName": "Polish",
      "interface": true,
      "subtitles": true,
      "voice": true
    }
  ],
  "systemRequirements": [
    {
      "id": "5b3382c7-8117-4526-865a-c8bf12946582",
      "operatingSystem": "PS",
      "deviceProcessor": "Pentium 4 or later",
      "deviceMemory": "2 GB RAM",
      "deviceStorage": "2.5 GB",
      "deviceGraphics": "NVIDIA GeForce GTX 260",
      "typeRequirements": "MINIMUM"
    }
  ]
}
```
**Post conditions:** вернуть систему в первоначальное состояние

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-21 | 12:27 | PASS | Дмитрий |  | 