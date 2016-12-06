starter-kit
========================

Разработка frontend

## Зависимости
- Node.js 4.5.0+
- Gulp 3.8+

## Установка Gulp
```bash
$ npm install --global gulp-cli
```

## Установка
Перейти в корневую папку проекта, запустить
```bash
$ npm i
```

## Запуск
Запускает локальный сервер и следит за обновлениями файлов(watcher)
```bash
$ gulp
```
Сборщик(минификатор)
```bash
$ gulp build
```

## Структура проекта
> assets/**/*.{jade, js(es6), scss} - исходники

> assets/blocks/*.{jade, js(es6), scss} - независимые блоки

> public/**/*.{html, js(es5), css} - сборка

> public/fonts - шрифты

> public/node_modules/* - сторонние библиотеки для frontend

## Работа с изображениями
> assets/images/* - загружать изображение 2x(для ретины)

на выходе получаются
> public/images/2x/* - оптимизированное изображение 2x(для ретины)

> public/images/1x/* - оптимизированное изображение 1x

Если исходное изображение не для ретины, загружать сразу в public/images/2x/*