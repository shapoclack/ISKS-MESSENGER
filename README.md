# Мессенджер с функцией регистрации
Этот проект представляет собой мессенджер с функцией регистрации, который состоит из двух частей: серверной части (ISKS BACK) и клиентской части (ISKS WEB). Ниже приведены инструкции для запуска проекта в двух режимах: с функцией валидации и без нее.

## Запуск с функцией валидации
Для запуска мессенджера с функцией регистрации, выполните следующие шаги:
```
1. Скачайте архив, содержащий папки "ISKS BACK" и "ISKS WEB".
2. Распакуйте архив в любое удобное для вас место.
3. Откройте папку "ISKS BACK" в любой интегрированной среде разработки (IDE) с встроенной поддержкой JDK версии 11+ (рекомендуется использовать IntelliJ IDEA).
4. Подключите базу данных, открыв файл "application.properties" в папке "resources". Рекомендуется использовать СУБД MySQL. При необходимости подключения другой СУБД, вам придется добавить соответствующие зависимости в файл "pom.xml".
5. Загрузите все зависимости, указанные в файле "pom.xml".
6. Запустите серверную часть, выполните метод "main" в классе "IsksApplication".
7. Откройте папку "ISKS WEB" (рекомендуется использовать Visual Studio Code).
8. Запустите команду "npm install" с помощью Node.js для установки всех зависимостей.
9. Выполните команды "npm install axios" и "npm install sockjs" для установки дополнительных зависимостей.
10. Запустите клиентскую часть, выполните команду "npm run start".
```
## Запуск без функции валидации
Если вы хотите запустить мессенджер без использования функций валидации, следуйте приведенным ниже инструкциям:
```
1. Скачайте архив, содержащий папки "ISKS BACK" и "ISKS WEB".
2. Распакуйте архив в любое удобное для вас место.
3. Скопируйте классы "WebSocketConfig", "MainController", "Message", "Status", "IsksApplication" и файл "pom.xml" в отдельную папку.
4. Откройте эту папку в любой интегрированной среде разработки (IDE) с встроенной поддержкой JDK версии 11+ (рекомендуется использовать IntelliJ IDEA).
5. Запустите серверную часть, выполните метод "main" в классе "IsksApplication".
6. Откройте папку "ISKS WEB" (рекомендуется использовать Visual Studio Code).
7. Удалите компоненты "Login.jsx" и "Register.jsx".
8. Удалите маршруты "Login" и "Register" из файла "App.js".
9. Запустите команду "npm install" с помощью Node.js для установки всех зависимостей.
10. Выполните команду "npm install sockjs" для установки дополнительной зависимости.
11. Запустите клиентскую часть, выполните команду "npm run start".
```
Теперь вы можете использовать мессенджер с функцией регистрации или без нее, в зависимости от выбранного режима запуска. Удачного использования!
