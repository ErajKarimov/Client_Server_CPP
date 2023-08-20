# Тестовое задание "Client_Server_Infotecs"

"Client_Server_Infotecs" - это клиент-сервер. Проект состоит из заголовочных файлов `Network.hpp`, `Client.hpp` и `Server.hpp`, а также файлов с исходными кодами `main_server.cpp` и `main_client.cpp`. Используется C++20.

## Описание файлов

### Network.hpp

Класс `Network` нужен для работы с сокетами и сетевыми операциями. Он содержит методы для создания сокета, отправки и чтения данных, прослушивания сокета и принятия подключений. Создал для упрощения работы с сетью.

### Server.hpp

Класс `Program2` реализует серверную часть. Внутри происходит привязка сокета к порту и прослушивания входящих подключений. Сервер принимает подключения, читает данные и обрабатывает их.

### Client.hpp

Класс `DataProcessor` реализует клиентскую часть. Обрабатывает пользовательский ввод и данные, отправляя их в `Program2`.

### main_server.cpp

Запускает сервер. Внутри создаётся объект `Program2`, который выполняет запуск сервера.

### main_client.cpp

Запускает клиента. Внутри создаётся объект `Program1`, который использует два потока для выполнения методов `processInput` и `processData`.

## Сборка проекта

Для сборки проекта требуется CMake версии >= 3.23 и стандарта C++20. Команды для сборки проекта:

```shell
mkdir build
cd build
cmake ..
make
```

Это создаст два исполняемых файла `client` и `server`, которые нужно запустить.

## Автор

Проект "Client_Server_Infotecs" разработал [Эрадж](https://github.com/ErajKarimov).
