# Postman: легкий старт в автоматизации тестирования API

## Предварительные требования

1. **Postman  :rocket:**

   Установите Postman, если у вас его ещё нет. Скачать можно здесь:
   
   [Скачать Postman](https://www.postman.com/downloads/)
   
   Если у вас нет аккаунта в Postman, пожалуйста, создайте его.


2. **Коллекции и окружения**

   Все коллекции и окружения, которые будут показаны на мастер-классе, доступны по ссылке: https://www.postman.com/shurka-tester/workspace/masterclass-data/overview
   
   Рекомендуется добавить их в локально установленный Postman.
   
   ![image](https://github.com/user-attachments/assets/360082c1-98f2-435c-8dca-be04e45107e5)

   ![image](https://github.com/user-attachments/assets/c40f8524-ce7f-4183-be94-5c7316012807)


## Описание API

### Shop 🛍️

Shop — это открытое приложение, предназначенное для практики в тест-дизайне и работе с REST и SOAP запросами. Приложение симулирует обычный интернет-магазин, позволяя создавать, изменять, удалять товары, а также проверять изменения в базе данных.

:heavy_check_mark: **[Документация](https://okiseleva.blogspot.com/2020/06/shop-soap-rest.html)**

:heavy_check_mark: **[Shop UI](http://shop.bugred.ru/)**

:heavy_check_mark: **Shop REST API**: http://shop.bugred.ru/api/items/<название_метода>

### Users 👥

Users — это приложение, напоминающее телефонный справочник, которое предоставляет обширный функционал для управления задачами и взаимодействия с пользователями.

Основные возможности:

- Создание и назначение задач исполнителям
- Планирование задач с помощью cron-выражения
- Уведомления для исполнителей о задачах и дедлайнах
- Возможность отмечать задачи как выполненные или невыполненные
- Роль менеджера с полным доступом к задачам всех пользователей
- Просмотр и фильтрация пользователей
- Поддержка SOAP и REST API


:heavy_check_mark: **[Документация](https://okiseleva.blogspot.com/2017/04/users-soap-rest.html)**

:heavy_check_mark: **[Users UI](http://users.bugred.ru/)**

:heavy_check_mark: **Users REST API**: http://users.bugred.ru/tasks/rest/list (все методы имеют тип POST)

:heavy_check_mark: **Users WSDL**: http://users.bugred.ru/tasks/soap/WrapperSoapServer.php?wsdl


### GraphQL :stars:

:heavy_check_mark: **[Countries GraphQL](https://countries.trevorblades.com)**
  
  Countries GraphQL API предоставляет информацию о странах, континентах и языках. Поддерживает фильтрацию по таким полям, как код страны, валюта и континент. API позволяет выполнять структурированные запросы через GraphQL и
  предоставляет данные о штатах/провинциях и AWS-регионах для каждой страны.
  
  Дополнительная информация доступна на [GitHub](https://github.com/trevorblades/countries).
  
:heavy_check_mark: **[Star Wars API](https://swapi-graphql.netlify.app/.netlify/functions/index)**

  SWAPI GraphQL API предоставляет обширную информацию о вселенной Star Wars, включая данные о планетах, космических кораблях, персонажах, фильмах и т.д.

  Более подробную информацию можно найти по [ссылке](https://studio.apollographql.com/public/star-wars-swapi/variant/current/home).
  

### WebSocket :speech_balloon:

:heavy_check_mark: **[WebSocket API BitMEX](wss://ws.bitmex.com/realtime)**

WebSocket API BitMEX обеспечивает потоковые данные в реальном времени для пользователей, включая информацию о сделках, книгах ордеров, котировках и изменениях в позициях. Он позволяет подписываться на определенные каналы, получая обновления без задержек. Это API оптимально подходит для высокочастотной торговли, так как обеспечивает быструю передачу данных и позволяет мгновенно реагировать на рыночные изменения. API также поддерживает аутентифицированные запросы для получения данных аккаунта и ордеров.

Для подробностей посетите [страницу WebSocket API](https://www.bitmex.com/app/wsAPI).

### gRPC :arrows_counterclockwise:

gRPC API, представленный в репозитории [shinkai-tester/gRPCServer](https://github.com/shinkai-tester/gRPCServer), предназначен для управления данными пользователей. Он позволяет выполнять операции по добавлению, поиску, обновлению и удалению пользователей. API поддерживает следующие методы:

- **AddPerson**: добавление нового пользователя.
- **FindPersonByName**: поиск пользователя по имени.
- **FindPersonById**: поиск пользователя по идентификатору.
- **UpdatePerson**: обновление информации о пользователе.
- **DeletePerson**: удаление пользователя из системы.

Для получения инструкций по настройке и запуску сервиса, ознакомьтесь с [README.md](https://github.com/shinkai-tester/gRPCServer/blob/main/README.md).


