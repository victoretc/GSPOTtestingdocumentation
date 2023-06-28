### Games community
#### PATCH comments

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/core/system_requirement/eba291a9-135d-4693-a0b7-525b27346b74/

**Type:** API

**Preconditions**: 
[Авторизоваться][a].

[a]: https://github.com/1fvwka/GSPOTtestingdocumentation/blob/main/Autorization.md

 **STR**

**1.Создать** новый запрос

**2.Выбрать** метод PATCH для Request

**3.Ввести URL:** https://games.alpha.g-spot.website/api/v1/core/system_requirement/eba291a9-135d-4693-a0b7-525b27346b74/

**4.Выбрать вкладку** Body=>Raw=>JSON

**5.Ввести данные** в окно ввода Body 
```json 
{
  "operatingSystem": "LINUX",
  "deviceProcessor": "string",
  "deviceMemory": "string",
  "deviceStorage": "string",
  "deviceGraphics": "Batman",
  "typeRequirements": "MINIMUM"
}
 ```
 **6.Нажать  "Send"**

 **Expected Result:**
 Server response: status code: 200 - OK
```json
{
  "id": "eba291a9-135d-4693-a0b7-525b27346b74",
  "operatingSystem": "LINUX",
  "deviceProcessor": "string",
  "deviceMemory": "string",
  "deviceStorage": "string",
  "deviceGraphics": "Batman",
  "typeRequirements": "MINIMUM"
}
```
**Post conditions:** вернуть систему в первоначальное состояние

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-21 | 12:00 | PASS | Дмитрий |  | 