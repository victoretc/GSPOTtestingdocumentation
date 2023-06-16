### Games community
#### Post comments

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/core/product/

**Type:** API

**Preconditions**: 
1. Запустить Postman
2. Выбрать пункт Autorization
3. Выбрать Type: Basic Auth
4. Авторизоваться : Username tester, Password tester


 **STR**
1.Создать новый запрос
2.Выбрать метод POST для Request
3.Ввести URL: https://games.alpha.g-spot.website/api/v1/core/product/
4.Выбрать вкладку Body=>Raw=>JSON
5.Ввести данные в окно ввода Body 

`{
  "name": "string",
  "developersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "publishersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "description": "string",
  "about": "string",
  "age": 2147483647,
  "adult": "string",
  "type": "GAMES",
  "systemRequirements": [
    {
      "operatingSystem": "LINUX",
      "deviceProcessor": "string",
      "deviceMemory": "string",
      "deviceStorage": "string",
      "deviceGraphics": "string",
      "typeRequirements": "MINIMUM"
    }
  ],
  "langs": [
    {
      "languageName": "string",
      "interface": true,
      "subtitles": true,
      "voice": true
    }
  ],
  "socials": [
    {
      "type": "FACEBOOK",
      "url": "string"
    }
  ],
  "productOffer": {
    "offer": {
      "createdBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
      "isActive": true,
      "products": [
        "3fa85f64-5717-4562-b3fc-2c963f66afa6"
      ],
      "price": {
        "amount": "string",
        "currency": "RUB",
        "createdBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "updatedBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
      }
    },
    "createdBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
  },
  "genres": [
    "string"
  ]
}`
 
 **4.Нажать  "Send"**

 **Expected Result:**
 Server response: status code: 201 - Created

`{
  "name": "string",
  "developersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "publishersUuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "description": "string",
  "about": "string",
  "age": 2147483647,
  "adult": "string",
  "type": "GAMES",
  "systemRequirements": [
    {
      "operatingSystem": "LINUX",
      "deviceProcessor": "string",
      "deviceMemory": "string",
      "deviceStorage": "string",
      "deviceGraphics": "string",
      "typeRequirements": "MINIMUM"
    }
  ],
  "langs": [
    {
      "languageName": "string",
      "interface": true,
      "subtitles": true,
      "voice": true
    }
  ],
  "socials": [
    {
      "type": "FACEBOOK",
      "url": "string"
    }
  ],
  "productOffer": {
    "offer": {
      "createdBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
      "isActive": true,
      "products": [
        "3fa85f64-5717-4562-b3fc-2c963f66afa6"
      ],
      "price": {
        "amount": "string",
        "currency": "RUB",
        "createdBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "updatedBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
      }
    },
    "createdBy": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
  },
  "genres": [
    "string"
  ]
}`

**Post conditions:** вернуть систему в первоначальное состояние

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-16 | 19:04 | FAIL | Дмитрий | https://trello.com/c/M1wexo2T | 