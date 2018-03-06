# Stream.Helper
Решение для удаленной работы со стримом (Например: Управление музыкой). Скрипт довольно гибкий и заточен под расширение функционала (Добавление новых модулей).
![2018-03-06_13-54-20](https://user-images.githubusercontent.com/10038023/37031128-4dda86a0-2146-11e8-869d-6f1f6658291b.png)

# Функционал
* Управление медиа во вкладках (Из коробки поддерживается: vk.com (Музыка), di.fm, twitch.tv, donatepay.ru). 
* Из коробки можно создавать свои виджеты не затрагивая ноду.

# ToDo
* Добавить поддержку donationalerts.ru, youtube.com, универсальный обработчик видео и аудио на любом сайте.

# Пример
Ознакомится с примером можно по ссылке: [https://klybok.net:3001/](https://klybok.net:3001/)

# Установка
В папке для установки выполните команды:
```
# git clone git@github.com:IvanDanilov/Stream.Helper.git .
# npm install
```
В файле ___index.js___ укажите путь к SSL сертификату (___const https___). Для запуска сервера выполните команду (сервер займет 3000 (http) и 3001 (https) порты):
```
# npm install forever
# forever start index.js
```
или
```
# node index.js
```
В файлах __./public/js/remote.js__ (var url) и __./public/index.html__ (script.src) укажите свой домен.
При внесении правок в файл __./public/js/app.js__ выполните команду:
```
# gulp
```
