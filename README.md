# Инструкция по запуску
## 1. Склонируйте данный репозиторий в любую директорию на вашей системе:
```shell
cd /path/to/dir
git clone https://github.com/cutlery47/message_bot_test_task.git
```
## 2. Получите у @BotFather аутентификационный токен для бота. Бота можете назвать произовально.  
## 3. В основной директории (где лежит compose-файл) создайте .env файл со следующими параметрами:
1. MESSAGE_SERVICE_PORT=... (Номер порта, на котором будет слушать приложение)
2. PROXY_PORT=... (Номер порта, на котором будет слушать прокси-сервер, рекоммендуется ставить такое же значение, что наверху)
3. MONGO_PORT=... (Номер порта, на котором будет слушать MongoDB, рекоммендуется 27017)
4. MONGO_DATABASE=... (Идентификатор базы данных MongoDB, произвольный)
5. MONGO_COLLECTION=... (Идентификатор коллекции MongoDB, произвольный)
6. BOT_TOKEN=... (Полученный токен бота)
## 4. Задеплойте приложение на локальной машине:
Из директории, где лежит compose-file пропишите:
```shell
docker compose build
docker compose up
```

