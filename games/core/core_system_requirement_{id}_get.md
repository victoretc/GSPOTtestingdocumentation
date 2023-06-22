### Games community
#### GET comments

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/core/system_requirement/eba291a9-135d-4693-a0b7-525b27346b74/

**Type:** API

**Preconditions**: 
[Авторизоваться][a].

[a]: https://github.com/1fvwka/GSPOTtestingdocumentation/blob/main/Autorization.md

 **STR**

**1.Создать** новый запрос

**2.Выбрать метод** GET для Request

**3.Ввести URL** https://games.alpha.g-spot.website/api/v1/core/system_requirement/eba291a9-135d-4693-a0b7-525b27346b74/

**4.Нажать:** "Send"

 **Expected Result:**
 Server response: status code: 200 - OK
```json
{
  "id": "eba291a9-135d-4693-a0b7-525b27346b74",
  "operatingSystem": "WINDOWS",
  "deviceProcessor": "Pentium 4 or later",
  "deviceMemory": "2 GB RAM",
  "deviceStorage": "2.5 GB",
  "deviceGraphics": "NVIDIA GeForce GTX 260",
  "typeRequirements": "MINIMUM"
}
```
**Post conditions:** вернуть систему в первоначальное состояние

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-21 | 11:45 | PASS | Дмитрий |  | 