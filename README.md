Л.р. 6 ­ организация параллельной обработки запросов на сервере с помощью мультиплексирования Модификация программы из Л.р. 5. Модифицировать сервер для организации параллельного обслуживания нескольких клиентов с помощью мультиплексирования (select, pselect, poll).

Использование:

Сомпилировать client.c с помощью gcc (с параметром -std=c99): gcc client.c -std=c99 -o client
Сомпилировать server.c с помощью g++ (с параметром -std=c++0x): g++ server.c -std=c++0x -o server
Для запуска программы в режиме сервера: ./server <-u> host port
Для запуска программы в режиме клиента: ./client <-u> host port ./file_path
В середине посылки данных отправляется срочные данные (для tcp). Данный факт отображается и на клиенте и на сервере.
