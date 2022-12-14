# gulp-wordpress

Сборка для разработки тем на Wordpress и Woocommerce

## Файловая структура

- dist  - Папка с собранными файлами
- src - Папка с исходными файлами
- functions - Папка с доп функциями Wordpress
- tempaltes - Папка с шаблонами компонентов Wordpress

## Обработка файлов в сборке

### Стили

- SASS компилятор
- Минификация стилей (при билде сборки)
- Autoprefixer (при билде сборки)
- Группирование Media запросов

### Скрипты

- Поддержка ES модулей
- Минификация скриптов 


### Шрифты

- Автоматическая конвертация шрифтов из одного формата во все

## Режимы работы

- dev (для использования просто пишем в терминал gulp)
- build (пишем в терминал gulp --build)

## Структура сборки

Для удобства все что касается gulp вынесено в отдельную папку **src/gulp**

Папка **config** отвечает за настройку путей для папок где находятся у куда конвертируются файлы

Папка **task** отвечает за задачи которые выполняет сборка

## Структура папок в сборке

### Папка config

- path.js - Настройка путей для конвертации файлов в режиме dev и build
- plugins.js - Плагины которые используются в большинстве задач, вынесены отдельно для удобства экспорта

### Папка tasks

- clean.js - отчиска папок dist от прошлых файлов
- copy.js - Копирование файловв dist
- fonts.js - Конвертация шрифтов
- images.js - Работа с картинками
- scripts.js - Работа со скриптами
- scss.js - Работа со scss Файлами

## Используемые плагины

- gulp-fonter
- gulp-ttf2woff2
- webpack-stream
- gulp-sass
- gulp-autoprefixer
- gulp-group-css-media-queries
- gulp-clean-css
- gulp-rename
- gulp-replace
- gulp-plumber
- gulp-notify
- gulp-if



