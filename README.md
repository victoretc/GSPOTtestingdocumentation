# GSpot - тестовая документация

**Инструкция**

1. Сделать Fork в свой репозиторий <details><summary>Скриншот</summary>![Fork](src/img/fork_example.png)</details>
2. Внести правки в файл/файлы
3. Отправить Pull request в основной репозиторий (с которого сделан Fork)
4. Изменения будут внесены после их одобрения владельцем основного репозитория.


**Структура документации**
* frontend - тестовая документация, относящаяся к frontend
* users, games, payments, channels - тестовая документация backend сервисов
    - Структура директрия внутри сервиса повторяет структуру api запросов.
Название ручки = название папки для группы запросов проверяющих её.
    - В название тест-кейса содержит positive или negative.
    - Метод пишется в названии файла в конце (get, post, delete и т.д.)
    - Games/reference/reference_genre_create/positive_standard-name_get.md - тест-кейс backend-сервиса games для проверки genre методом get.
* src - для изображений и прочего

Информация по авторизации предоставляется по [ссылке](https://github.com/nastyaist/GSPOTtestingdocumentation/blob/main/Authorization%20data.md).