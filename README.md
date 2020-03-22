# webpack
webpack setup
---
Создать папку 'webpack'

Ctrl+` - открыть консоль

`git init` - инициализировать репозиторий

создаём репозиторий на github

пишем в консоль, чтоб прицепиться к гитхабу:
```
git remote add origin https://github.com/DokSna/webpack.git

git push -u origin master
```
Прицепиться к пустому репозиторию на гитхабе не получилось, поэтому использовал другой вариант.

Создал репозиторий на гитхабе и склонировал себе на комп.

С git разобрался, можно приступать к webpack.

Добавить файл .gitignore

В консоли:

`npm -v` - проверили версию npm, версия есть значит Node.js установлен, можно продолжать.

## Инициализация вебпака

В консоли:

`npm init`

далее нужно следовать тому, что скажет npm либо просто набрать

`npm init  -y`

в таком случае, неприхотливый нпм согласиться со всем не раздумывая.

Появился файл *package.json*

## Установка webpack-dev-server

В консоли:

`npm install webpack webpack-cli webpack-dev-server path --save-dev`

## По умолчанию, Webpack (начиная с 4-й версии) не требует никакой настройки, если вы соблюдаете эти правила:

* точкой входа вашего приложения является ./src/index.js
* вывод (output) размещается в ./dist/main.js
* Webpack работает в production mode (режим производства)

Создадим папку *src* и файл *index.js*

В *package.json* скрипт test исправим на:
```json
"build": "webpack --mode production"
```
В консоли:

`npm run build` - и сгенерировалась папка *dist*, а в ней файл main.js

