# frontend-sandbox

Изучать всевозможные фреймворки и библиотеки удобно на примерах.
[frontend-sandbox-core](https://github.com/maestrow/frontend-sandbox-core) - это небольшая платформа для хостинга коллекции демонстрационных примеров frondtend-технологий.
frontend-sandbox - это шаблон для вашей новой коллекции примеров.


## Quick Start

- `git clone https://github.com/maestrow/frontend-sandbox . --depth=1`.
- В `bower.json`, в раздел `dependencies` добавьте зависимости на клиентские пакеты, которые планируете использовать. Например, `"jquery": ""`.
- `$ npm install` (1).
- `$ npm start`
- Укажите имя и описание вашего пакета (а также другую информацию) в `package.json`.

Модули примеров находятся в `frontend/modules`.
За дополнительной информацией см. https://github.com/maestrow/frontend-sandbox-core.


## Демонстрационные модули

- Демонстрационные модули оформляются в виде отдельной папки и располагаются в `frontend/modules`.
- На главной страничке (http://localhost:4000) автоматически формируется список всех модулей.
- Модуль может состоять из файла макета `<ИмяМодуля>.html`, других `.html`-файлов и `.js`-файлов. Наличие файлов опционально.
- При переходе по адресу модудя (`http://localhost:4000/show/<ИмяМодуля>`) содержимое файла `<ИмяМодуля>.html` будет вставлено в тэг `<body>` общего макета `views\master.ejs`.
А `.js`-файлы, соответственно будут добавлены в теги `<script>`


## Примечания

- (1) В Windows необходимо выполнять эту команду из git-bash. Это необходимо для корректного срабатывания комманды
установки пакета `frontend-sandbox` из репозитория (по данному поводу см. комментарии в [https://github.com/npm/npm/issues/2478]()).
