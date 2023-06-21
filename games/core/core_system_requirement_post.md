### Games community
#### Post comments

**Тестовые данные:** https://games.alpha.g-spot.website/api/v1/core/system_requirement/

**Type:** API

**Preconditions**: 
[Авторизоваться][a].

[a]: https://github.com/1fvwka/GSPOTtestingdocumentation/blob/main/Autorization.md

 **STR**

1.Создать новый запрос

2.Выбрать метод POST для Request

3.Ввести URL: https://games.alpha.g-spot.website/api/v1/core/system_requirement/

4.Выбрать вкладку Body=>Raw=>JSON

5.Ввести данные в окно ввода Body 
```json 
{
  "operatingSystem": "LINUX",
  "deviceProcessor": "<Pentium 2 or later>",
  "deviceMemory": "<2 GB RAM>",
  "deviceStorage": "<1 GB>",
  "deviceGraphics": "<Radeon 9600>",
  "typeRequirements": "MINIMUM",
  "id": "<uuid>"
}
 ```
 **4.Нажать  "Send"**

 **Expected Result:**
 Server response: status code: 201 - Created
```json
	

{
  "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "operatingSystem": "LINUX",
  "deviceProcessor": "Pentium 2 or later",
  "deviceMemory": "2 GB RAM",
  "deviceStorage": "1 GB",
  "deviceGraphics": "Radeon 9600",
  "typeRequirements": "MINIMUM"
}

```
**Post conditions:** вернуть систему в первоначальное состояние

Автор: Дмитрий

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-06-21 | 11:30 | FAIL | Дмитрий | https://trello.com/c/Uw0ssDdt | 