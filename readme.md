Замечания по уроку 6:
1) Функция showNews выглядит чужой в app.js. Неплохо было бы вынести ее.
2) Не стоит закрывать корень, пусть часть проекта будет открытой.
3) Лучше не передавать req и res во ввнешние функции из роутинга. Пусть мы вычленим все данные, которые нам нужны и передадим их внешней функции, а получив результат, сформируем ответ клиенту.
4) Вижу что часть логики повторяется. Предлагаю пересмотреть api ресурса, особенно в свете вебинара по REST API.
5) Проблема с getNews, проверьте валидацию входных данных.
Исправлено:
1 - 3. 
По п.5 есть вопрос: о какой именно проблеме идет речь: https://github.com/webmaza75/try_nodejs/blob/master/ira_lesson7/lib/getnews.js#L8 (получение новостей для БД) 
или методе получения новостей из выбранной категории: https://github.com/webmaza75/try_nodejs/blob/master/ira_lesson7/lib/pool-server.js#L9 ?
