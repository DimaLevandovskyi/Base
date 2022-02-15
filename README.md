# Base
Базовая сборка для Shopify/Shopify+.
1. Клонируем сборку
2. Устанавливаем модуля в терминале проекта (комманда npm i). Для этого нужно установить изначально Node.js. Link: https://nodejs.org/uk/
3. Изменить конфиг под свой (config.yml) 
  development:
    password: 'your_password'
    theme_id: "theme_id"
    store: "store_link"
4. Запускаем сборку коммандой npm run dev. Открываем тему коммандой theme open.

***** Стили и скрипты *****
Находятся в папке src. 

Скрипты - src/scripts. Обертка-файл custom.js, куда мы подключаем все второстепенные скрипты. Главный же файл - index.js, его мы не трогаем.
Эти скрипты билдятся в файл scripts.bundle.js, который 
находится в папке "assets". У папке scripts можно создавать свои дополнительные папки.

Стили - src/styles. Главный файл custom.scss, куда мы подключаем все второстепенные стили. Эти стили билдятся в файл styles.css, который 
находится в папке "assets". У папке styles можно создавать свои дополнительные папки.


***** Liquid srtucture *****
Папка section - находятся все секции магазина
Папка snippets - находятся все снипеты магазина
Папка layout - theme.liquid. Layout-files, сюда же закидывать checkout.liquid.
