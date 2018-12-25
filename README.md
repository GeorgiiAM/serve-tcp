# server-tcp
Создать клиент-серверное приложение на C# (WinForms или WPF или ASP.NET MVC).
- клиент TCP
- сервер TCP
- на клиенте можно выбрать какие данные отправлять
- клиент посылает ASCII данные серверу. Сервер проверяет корректность данность и если они корректны – обрабатывает их (парсит).
- после приема данных сервер посылает клиенту ответ: ACK или NACK. (ACK – все успешно, NACK – получена ошибка). Без кодов ошибок.
- если получен NACK, клиент повторно отправляет данные. Максимальное число повторов – 3.
- на клиенте и сервера должна выводится информация об отправке/получении данных
