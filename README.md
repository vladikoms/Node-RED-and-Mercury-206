# Node-RED-and-Mercury-206
Пример обработки данных счетчика эл. энергии Меркурий 206 PRSN в Node-RED. Для связи со счетчиком использован дешевый переходник "USB to RS485" c aliexpress. 

![screenshot of sample](https://github.com/vladikoms/Node-RED-and-Mercury-206/blob/main/01.jpg)

В репозитории загружен файл потока Node-RED <B>flows.json</B>. Дополнительно необходимо установить ноды <B>node-red-node-serialport</B> и <B>node-red-dashboard</B> через меню Node-RED: <B>Menu > Manage palette > Install</B>

![screenshot of sample](https://github.com/vladikoms/Node-RED-and-Mercury-206/blob/main/Node_red.jpg)

Для работы с произвольным счетчиком Меркурий 206 необходимо заменить адрес счетчика в запросах sendReq. Пример:

var serial = 42356415;

42356415 - серийный номер счетчика (сетевой адрес), указанный на лицевой стороне прибора.

<h2> Благодарности </h2>

Выражаю благодарность Александру Лифанову и Александру Воронину OOO «Сименс» за любезно предоставленный образец кода.

<h2> Полезные ссылки </h2>

1. Как соединить Simatic IOT2040 и электросчетчик «Меркурий». https://zen.yandex.ru/media/id/5d0cd52d70a11800afed36e2/kak-soedinit-simatic-iot2040-i-elektroschetchik-merkurii-5d0d167ba346fd00affa67be

2. Протокол обмена однофазных счетчиков Меркурий 200, 201, 203 (кроме Меркурий 203.2TD), 206. https://www.incotexcom.ru/files/em/docs/mercury-protocol-obmena-1.pdf

3. Node-red-node-serialport https://flows.nodered.org/node/node-red-node-serialport

4. Node-red-dashboard https://flows.nodered.org/node/node-red-dashboard
