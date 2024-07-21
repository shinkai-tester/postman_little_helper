# Postman: легкий старт в автоматизации тестирования API

## Предварительные требования

### Установка необходимого ПО

1. **Postman  :rocket:**

   Установите Postman, если у вас его ещё нет. Скачать можно здесь:
   
   [Скачать Postman](https://www.postman.com/downloads/)
   
   Если у вас нет аккаунта в Postman, пожалуйста, создайте его.

2. **Git :octocat:**

   Проверьте, установлен ли у вас Git, так как он понадобится для клонирования репозитория:
   
   [Скачать Git](https://git-scm.com/downloads)

3. **Docker :whale:**

   Docker необходим для запуска локальных серверов gRPC. Установите Docker, следуя этим инструкциям:
   
   - [Docker Desktop](https://www.docker.com/products/docker-desktop/)
   - [Установка Docker на Windows (GeeksforGeeks)](https://www.geeksforgeeks.org/how-to-install-docker-on-windows/)
   - [Установка Docker Desktop на Windows (Medium)](https://medium.com/@meghasharmaa704/install-docker-desktop-on-windows-ce0f2f987bfc)

## Настройка рабочего окружения :wrench:

### Клонирование репозитория

   Клонируйте репозиторий с помощью следующей команды (например, в Git Bash):
```bash
git clone https://github.com/shinkai-tester/postman_little_helper.git
```

## REST и SOAP API

В репозитории вы найдете коллекции Postman для работы с REST и SOAP API:

### Shop 🛍️

- **Коллекция:** `Shop.postman_collection`
- **Окружение:** `Shop_environment`
- **Документация:** [Shop API](https://okiseleva.blogspot.com/2020/06/shop-soap-rest.html)
- **Интерфейс:** [Shop UI](http://shop.bugred.ru/)

### Users 👥

- **Коллекции:** `Users.postman_collection`, `Users_SOAP.postman_collection`
- **Окружение:** `Users_environment`
- **Документация:** [Users API](https://okiseleva.blogspot.com/2017/04/users-soap-rest.html)
- **Интерфейс:** [Users UI](http://users.bugred.ru/)

## GraphQL, WebSocket, и gRPC

После мастер-класса рекомендуется посетить публичный воркспейс в Postman, где вы найдете коллекции для GraphQL, WebSocket и gRPC:

[Посмотреть воркспейс](https://www.postman.com/shurka-tester/workspace/masterclass-data/overview)

### GraphQL :stars:

- [Countries GraphQL](https://countries.trevorblades.com) — подробности на [GitHub](https://github.com/trevorblades/countries)
- [Star Wars API](https://swapi-graphql.netlify.app/.netlify/functions/index) — подробности по [ссылке](https://studio.apollographql.com/public/star-wars-swapi/variant/current/home)

### WebSocket :speech_balloon:

- [WebSocket Echo Server](wss://echo.websocket.org) — подробнее на [WebSocket.org](https://websocket.org/tools/websocket-echo-server)

### gRPC :arrows_counterclockwise:

- **Запуск gRPC сервера** — используйте следующую команду:
```bash
docker run -it --rm -p 9000:9000 -p 9001:9001 moul/grpcbin
```


Сервис будет доступен по адресам `grpc://localhost:9001` и `grpc://localhost:9000` (без TLS, незащищенное соединение).

Подробности о сервисе: [GitHub grpcbin](https://github.com/moul/grpcbin), альтернатива: [GitHub k6-grpcbin](https://github.com/grafana/k6-grpcbin).

