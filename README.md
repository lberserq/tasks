# Задания с репозиториями

Все задания должны храниться в git-репозитории (например, GitHub), включать в себя тесты (по выбору), интеграцию с CI (например, Travis), выгрузку анализа покрытия (например, coveralls/codecov), работу с базой данных.

Интерфейс ко всем заданиям не обязателен (по желанию), на оценку не повлияет.

Сторонние библиотеки (вспомогательные) использовать можно. Например, для реализации WebSocket, oAuth, роутинга, и т.д.

## 4 курс и магистры
1. **Шейдаев Вадим**
 
 Чат с авторизацией через соц.сети, websocket, тесты
 Xранение — MongoDB.
 Команды (через !команда) — поиск в гугле и выдача первого результата с заголовком, выдача первого абзаца описания из вики по названию статьи.
 
 Репозиторий — ???.

2. **Глейзерман Светлана**
 
 Чат, хранение — MariaDB.
 Команды — регистрация, авторизация, кик пользователя, рассылка сообщений всем, отправка приватных сообщений.
 Тесты должны в т.ч. эмулировать клиента, то есть проходить процедуру регистрации, писать, убеждаться, что получают сообщения.
 
 Репозиторий — ???.

3. **Беляев Михаил**
 
 Тасклисты, с регистрацией и возможностью шаринга.
 У тасклиста есть владелец (создатель), который может выдавать другим пользователям доступ (или запрещать).
 В тасклисте есть название и список тасков, которыми может управлять любой пользователь с доступом
 У таска несколько статусов завершённости (список заранее задан, 4-5, придумайте) и комментарии от пользователей
 БД — MongoDB.
 Регистрация — POST (или PUT)-запрос, обмен данными в тасклисте — WebSocket. Тесты.

 Дополнительно можно приделать авторизацию через гитхаб (или что-нибудь другое), но это по желанию. Либо можно приделать её же вместо регистрации вообще.
 Если делать через гитхаб, то можно и тасклисты к репозиториям привязать, но это, опять же, абсолютно не обязательно — по желанию. См https://waffle.io/, например.
 
 Репозиторий — ???.

4. **Жуков Владимир**
 
 «Морской бой», по WebSocket, авторизация через любую соцсеть по выбору (или через GitHub/Google/что угодно). MongoDB (сам попросил). Историю игр и ходов хранить.
 По человеку считать статистику выигрышей-проигрышей. Обязательна только серверная часть, интерфейс — по желанию.
 Должна быть возможность закрыть окно и открыть его заново, вернувшись к игре, а так же вести несколько игр одновременно.
 Только серверная часть, так что на практике это значит что надо хранить и передавать по запросу состояние.
 
 Репозиторий — https://github.com/GoldenMan123/battleship

 Сервер — http://mks1.cs.msu.ru:9090/

5. **Закляков Роман**
 
 «Крестики-нолики», на бесконечном поле, по WebSocket, авторизация через любую соцсеть по выбору (или через GitHub/Google/что угодно). MongoDB (сам попросил). Историю игр и ходов хранить.
 По человеку считать статистику выигрышей-проигрышей. Обязательна только серверная часть, интерфейс — по желанию.
 Должна быть возможность закрыть окно и открыть его заново, вернувшись к игре, а так же вести несколько игр одновременно.
 Только серверная часть, так что на практике это значит что надо хранить и передавать по запросу состояние.
 
 Репозиторий — ???.
 
6. **Луценко Юрий**

 Планировщик событий.
 Пользователи, с регистрацией (логин-пароль).
 События привязываются к дате и времени, могут быть определённой продолжительности. События могут пересекаться (тут никакой хитрой логики делать не надо).
 Пользователи могут создавать списки событий, которые могут быть публичные (доступны всем), и приватные (доступны всем, у кого есть общий токен).
 Пользователи могут отмечаться в событиях (придёт/не придёт/возможно придёт), с комментарием. На каждого пользователя комментарий один, но может быть обновлён.
 REST API для всех операций, WebSocket для получения обновлений по конкретному событию.
 Интерфейс не обязателен. БД — ~~любая не SQL, но база данных~~ выбрал MongoDB.
 
 Репозиторий — ???.

7. **Овчинников Дмитрий**

 Чат.

 БД: Redis. 

 Функциональность:
  1. Оправка сообщений всем участникам чата(broadcast)
  2. Регистрация новых пользователей
  3. Авторизация пользователей
  4. Удаление пользователей(только для админа)

  Репозиторий: https://github.com/ovchinnikov94/chat_nodejs

8. **Беляев Андрей Юрьевич**
 
 Простые «Шашки» (на 2 человек), по WebSocket, авторизация через любую соцсеть по выбору (или через GitHub/Google/что угодно). Историю игр и ходов хранить. Сервер должен верифицировать ходы и определять выигрыш.
 БД — любая, какой вы раньше не пользовались.
 
 По человеку считать статистику выигрышей-проигрышей. Обязательна только серверная часть, интерфейс — по желанию.
 
 Должна быть возможность закрыть окно и открыть его заново, вернувшись к игре, а так же вести несколько игр одновременно.
 Только серверная часть, так что на практике это значит что надо хранить и передавать по запросу состояние.
 
 Репозиторий — ???.

9. **Хамитов Камиль**
 
 Анонимные заметки к профилю. Авторизация через любую соцсеть (например, ВК), авторизированные люди могут сохранять и изменять заметки ко всем и видеть свои заметки, но без отображения, от кого. Можно добавлять к каждому человеку несколько заметок, тогда он видит, что они от одного автора, (но не видит, от какого). На заметки можно отвечать как на цепочки обсуждений, но только автору и тому, кто их создал.
 Только серверная часть.
 БД — любая, какой вы раньше не пользовались.
 
 Репозиторий — ???.

## 3 курс
 1. **Маторин Николай**
 
 Хранилище файлов (можно только картинок). Авторизация через что угодно по выбору. 
 Файлы могут быть публичными и приватными (доступны только по ссылке-ключу, не индексируются), у них может быть описание и метки. Метки задаются внутри описания через `#метка`.
 Редактирование описаний можно не добавлять.
 У авторизированного пользователя должна быть возможность удалить свои файлы (все или по одному), а так же менять своим файлам состояние публичный/приватный (по одному).
 Через WebSocket — возможность (анонимно) следить за добавлением и удалением публичных файлов с определённой меткой (одной).
 Аналогично — возможность анонимно следить за добавлением и удалением публичных файлов с определённой меткой через long polling.
 На каждого пользователя — ограничение общего размера его файлов (настраиваемое в файле конфигурации).
 Только сервер, интерфейс не обязателен.
 БД — любая, какой вы раньше не пользовались.
 
 Репозиторий — ???.
 
 2. **Горбачев Даниил**
 
 Сервер скриншотов по переданной ему ссылке. Регистрация, авторизация, подтверждение аккаунтов администратором.
 Пользователям выдаются уникальные ключи доступа по логину-паролю. Ключи уже используются как токены в запросах.
 Интерфейсы команд на WebSocket и через REST API. По WebSocket приходят все изменения, включая те, которые совершены из REST API.
 Команды: сделать скриншот страницы, список всех скриншотов, удалить скриншот, удалить всё.
 Получаются сами картинки по GET по идентификатору (который не включает в себя имя пользователя).
 Дата взятия скриншота тоже записывается.
 Ограничение на количество скриншотов на одного человека (настраиваемое в конфиге, но одинаковое для каждого).
 БД — любая, какой вы раньше не пользовались.
 Сама операция взятия скриншота совершается в несколько строчек, смотреть в сторону phantomjs или обёрток над ним.
 
 Репозиторий — ???.
 

## 2 курс
 1. **Гурьев Николай**
  
  Новости. БД — ~~любая, какой вы раньше не пользовались~~ выбрал MongoDB.
  
  В БД есть:
  1. Аккаунты доступа — id, токен, описание. Интерфейса для добавления новых аккаунтов реализовывать не надо.
  2. Собственно, новости — дата публикации, статус (черновик/готово/опубликовано/удалено), ссылки на источники (список название-описание), текст (форматирование на сервере делать не надо, считаем что интерфейс позволяет html), журнал изменений состояния (все поля + дата изменения + id и описание автора).
 
  Операции по REST API — только для новостей: POST для создания, PUT для обновления, GET для получения и DELETE для удаления (ставит статус в «удалено» и скрывает новость). Авторизация через Bearer-токен в заголовке. Все операции, кроме GET опубликованных новостей, требуют авторизации. Плюс публичный GET для листинга последних N опубликованных новостей (по дате публикации, N — параметр) и ещё один приватный (требующий авторизации) — для листинга последних N новостей в любом статусе.
 
  По WebSocket — всем клиентам рассылаются все _публичные_ изменения (изменения при новом статусе «опубликовано» или просто нотификация об удалении новости при изменении состояния с «опубликовано» на любое другое)
  
 Репозиторий — ???.
