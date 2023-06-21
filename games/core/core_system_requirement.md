### Games community
#### GET comments

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/core/system_requirement/?limit=4&offset=2

**Type:** API

**Preconditions**: 
[Авторизоваться][a].

[a]: https://github.com/1fvwka/GSPOTtestingdocumentation/blob/main/Autorization.md

 **STR**

**1.Создать:** новый запрос

**2.Выбрать метод:** GET для Request

**3.Ввести URL:** https://games.alpha.g-spot.website/api/v1/core/system_requirement/?limit=4&offset=2

**4.Нажать:**  "Send"

 **Expected Result:**
 Server response: status code: 200 - OK
```json
{
  {
  "count": 8,
  "next": "https://games.alpha.g-spot.website/api/v1/core/system_requirement/?limit=4&offset=6",
  "previous": "https://games.alpha.g-spot.website/api/v1/core/system_requirement/?limit=4",
  "results": [
    {
      "id": "7a2275e2-083d-428a-9099-3b7889936d64",
      "operatingSystem": "PS",
      "deviceProcessor": "Pentium 4 or later",
      "deviceMemory": "2 GB RAM",
      "deviceStorage": "2.5 GB",
      "deviceGraphics": "NVIDIA GeForce GTX 260",
      "typeRequirements": "MINIMUM"
    },
    {
      "id": "08df6309-6b2a-4a88-8d49-7a9748a85f29",
      "operatingSystem": "WINDOWS",
      "deviceProcessor": "Pentium 4 or later",
      "deviceMemory": "2 GB RAM",
      "deviceStorage": "2.5 GB",
      "deviceGraphics": "NVIDIA GeForce GTX 260",
      "typeRequirements": "MINIMUM"
    },
    {
      "id": "dfb761a0-6e78-4d8f-8494-05578497da48",
      "operatingSystem": "PS",
      "deviceProcessor": "Pentium 4 or later",
      "deviceMemory": "2 GB RAM",
      "deviceStorage": "2.5 GB",
      "deviceGraphics": "NVIDIA GeForce GTX 260",
      "typeRequirements": "MINIMUM"
    },
    {
      "id": "b0e1a84c-8f87-4e9e-bace-3712b05de146",
      "operatingSystem": "WINDOWS",
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
| 2023-06-21 | 10:27 | PASS | Дмитрий |  | 