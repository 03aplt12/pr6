
## HTTP-сообщения
HTTP (HyperText Transfer Protocol) - это протокол прикладного уровня, который используется для обмена данными между клиентом и сервером в сети Интернет. HTTP-сообщения представляют собой синтаксически структурированные блоки данных, которые передаются между клиентом и сервером.

В HTTP-протоколе существуют два основных типа сообщений: запросы (HTTP request) и ответы (HTTP response). Рассмотрим каждый тип подробнее:

1. HTTP Запрос (HTTP Request):
   - Стартовая строка: Содержит метод запроса (GET, POST, PUT, DELETE и т.д.), целевой URI (Uniform Resource Identifier) и версию HTTP-протокола.
   - Заголовки (Headers): Заголовки содержат дополнительную информацию о запросе, такую как параметры авторизации, тип содержимого (Content-Type) и другие метаданные.
   - Тело (Body): Необязательное поле, используется для передачи данных в запросе. Обычно используется с методами POST или PUT.

2. HTTP Ответ (HTTP Response):
   - Стартовая строка: Содержит версию HTTP-протокола, статус код (например, 200 OK) и описание статуса.
   - Заголовки (Headers): Аналогично запросу, заголовки содержат дополнительную информацию об ответе, такую как тип содержимого, дата создания, сервер и др.
   - Тело (Body): Необязательное поле, содержит данные, переданные в ответе сервера, например, HTML-код страницы или данные в формате JSON.

HTTP-сообщения играют ключевую роль во взаимодействии клиента и сервера в Интернете. Они позволяют клиентам запрашивать ресурсы (например, веб-страницы) и получать ответы от серверов.
 
 ## HTTP методы
 
 Описание девяти основных HTTP методов, используемых для создания запросов к серверу:

1. GET: GET-запрос используется для получения данных с сервера по указанному URI. Он используется для получения ресурсов без изменения состояния сервера. GET-запросы могут содержать параметры запроса в URL для передачи дополнительной информации. Ответ сервера содержит запрошенные данные в теле ответа.

2. POST: POST-запрос используется для отправки данных на сервер для обработки. Обычно он используется для создания нового ресурса, отправки данных формы или загрузки файлов. Данные отправляются в теле запроса. Сервер может вернуть в ответе новый ресурс или подтверждение об успешном создании.

3. PUT: PUT-запрос используется для обновления ресурса на сервере. Он аналогичен POST-запросу, но используется для полного замещения существующего ресурса на сервере данными, указанными в теле запроса. Если ресурс не существует, он может быть создан. PUT-запрос также может использоваться для создания нового ресурса с определенным URI.

4. DELETE: DELETE-запрос используется для удаления ресурса на сервере по указанному URI. После выполнения этого запроса сервер должен удалить указанный ресурс. DELETE-запрос также должен быть идемпотентным, то есть повторное выполнение запроса не должно приводить к изменению состояния сервера.

5. PATCH: PATCH-запрос используется для частичного обновления ресурса на сервере. Он применяется для изменения только определенных полей или свойств ресурса, указанных в теле запроса. Другие поля ресурса остаются неизменными. PATCH-запрос обычно применяется, когда обновление целого ресурса не требуется.

6. HEAD: HEAD-запрос выполняет запрос заголовков ответа от сервера без тела ответа. Он используется, когда клиенту требуется только получить метаданные ответа, например, информацию о типе содержимого, дате изменения или размере ресурса. HEAD-запрос полезен для проверки статуса ресурса или получения информации о кэшировании.

7. OPTIONS: OPTIONS-запрос используется для получения информации о возможностях сервера. Сервер возвращает список поддерживаемых методов, заголовков и других свойств, что позволяет клиенту определить, какие операции можно выполнить над указанным ресурсом. OPTIONS-запрос полезен при разработке API или при определении возможностей сервера.

8. TRACE: TRACE-запрос используется для диагностики и отладки. Сервер возвращает весь полученный TRACE-запрос в теле ответа, что позволяет клиенту видеть, какие изменения происходят с запросом на протяжении его прохождения через различные прокси-серверы или промежуточные узлы.

9. CONNECT: CONNECT-запрос используется для установления "туннеля" к удаленному серверу, обычно для установки защищенного SSL/TLS-соединения. CONNECT-запрос выполняется прокси-сервером и устанавливает прямое соединение между клиентом и удаленным сервером.

Это основные HTTP методы, которые широко используются при создании запросов к серверу. Каждый из них имеет свою специфическую функцию и позволяет взаимодействовать с сервером в соответствии с нуждами приложения или сервиса.