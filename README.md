# Node-RED-and-Mercury-206
Пример обработки данных счетчика эл. энергии Меркурий 206 в Node-RED. Для связи со счетчиком использован "RS485 to USB adapter" c aliexpress.

![screenshot of sample](https://github.com/vladikoms/Node-RED-and-Mercury-206/blob/main/01.jpg)

В репозитории загружен файл потока Node-RED

![screenshot of sample](https://github.com/vladikoms/Node-RED-and-Mercury-206/blob/main/Node_red.jpg)

Для работы с произвольным счетчиком Меркурий 206 необходимо заменить адрес счетчика в запросах sendReq. Пример:

var serial = 42356415;

42356415 - номер счетчика (адрес), указанный на лицевой стороне счетчика. Этот адрес также можно увидеть в программе "Конфигуратор счетчиков "Меркурий"" > Настройка/параметры связи

<h1> Благодарности

Выражаю благодарность Александру Лифанову и Александру Воронину OOO «Сименс» за любезно предоставленный образец кода.

<h1> Полезные ссылки
  
1. Как соединить Simatic IOT2040 и электросчетчик «Меркурий». https://zen.yandex.ru/media/id/5d0cd52d70a11800afed36e2/kak-soedinit-simatic-iot2040-i-elektroschetchik-merkurii-5d0d167ba346fd00affa67be
