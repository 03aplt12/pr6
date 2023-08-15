# Activities
## 1. GET​/api​/v1​/Activities
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200
- Тело ответа (часть): 
```json
[
    {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-20T15:39:58.6485819+00:00",
    "completed": false
  },
  {
    "id": 2,
    "title": "Activity 2",
    "dueDate": "2023-06-20T16:39:58.6485838+00:00",
    "completed": true
  }
   ]
```

## 2. POST​/api​/v1​/Activities
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
- Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
    "id": 0,
  "title": "string",
  "dueDate": "2023-06-20T15:09:07.366Z",
  "completed": true
}
```
- Статус-код ответа: 200 успешный
- Тело ответа:
```json
{
    "id": 0,
  "title": "string",
  "dueDate": "2023-06-20T14:55:04.068Z",
  "completed": true
}
```
## 3. POST​/api​/v1​/Activities
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
- Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
    "id": 3076543234567808,
  "title": "string",
  "dueDate": "2023-06-23T14:14:04.856Z",
  "completed": true
}
```
- Статус-код ответа: 400 Ошибка запроса
- Тело ответа:
```json
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c9d9d71b0747ae44b2fb7dfdf4a1f86a-6ea44939824f9047-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 22."
    ]
  }
}
```
## 4. GET​/api​/v1​/Activities​/{55}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/55
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 404 не найден
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-30ac497f68cd154390cbfbeb94bbf531-e68444e20541ed4f-00"
}
```
## 5. GET​/api​/v1​/Activities​/{5}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/5
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-23T14:32:44.283Z",
  "completed": true
}
```
## 6. PUT​/api​/v1​/Activities​/{2}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/2
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 2,
  "title": "string",
  "dueDate": "2023-06-23T14:32:44.283Z",
  "completed": true
}
```
- Статус-код ответа: 200
- Тело ответа: 
```json
{
  "id": 2,
  "title": "string",
  "dueDate": "2023-06-23T14:32:44.283Z",
  "completed": true
}
```

## 7. PUT​/api​/v1​/Activities​/{3409876532}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/3409876532
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 3409876532,
  "title": "string",
  "dueDate": "2023-06-23T14:32:44.283Z",
  "completed": true
}
```
- Статус-код ответа: 404 Bad Request
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-3e095e4ca31e7749901dbb552e2677b9-a416630325d9754c-00",
  "errors": {
    "id": [
      "The value '3409876532' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 16."
    ]
  }
}
```
## 8. DELETE​/api​/v1​/Activities​/{33}
Описание запроса:
- HTTP-метод: DELETE
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/33
- Заголовки запроса:  -H  "accept: */*"
- Тело запроса: отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: отсутствует

# Authors

## 9. GET​/api​/v1​/Authors
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200
- Тело ответа (часть): 
```json
[
   {
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 2,
    "idBook": 1,
    "firstName": "First Name 2",
    "lastName": "Last Name 2"
  },
   ]
```
## 10. POST​/api​/v1​/Authors
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
- Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Статус-код ответа: 200 успешный
- Тело ответа:
```json
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
## 11. POST​/api/v1/Authors
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
- Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 34567876543890,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Статус-код ответа: 400 Ошибка запроса
- Тело ответа:
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-098ce66437dd7c40afaf4fbd153d45f8-ef21ae239d5b5a4e-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 20."
    ]
  }
}
```
## 12. GET​/api​/v1​/Authors​/authors​/books​/{21}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/21
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
[
  {
    "id": 70,
    "idBook": 21,
    "firstName": "First Name 70",
    "lastName": "Last Name 70"
  },
  {
    "id": 71,
    "idBook": 21,
    "firstName": "First Name 71",
    "lastName": "Last Name 71"
  },
  {
    "id": 72,
    "idBook": 21,
    "firstName": "First Name 72",
    "lastName": "Last Name 72"
  },
  {
    "id": 73,
    "idBook": 21,
    "firstName": "First Name 73",
    "lastName": "Last Name 73"
  }
]
```
## 13. GET​/api​/v1​/Authors​/authors​/books​/{8969909876543}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/8969909876543
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 400 ошибка запроса
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-4172d98ba180ba40a020220d0d477914-e60a9682557d124c-00",
  "errors": {
    "idBook": [
      "The value '8969909876543' is not valid."
    ]
  }
}
```
## 14. GET​/api​/v1​/Authors​/{7}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/7
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
{
  "id": 7,
  "idBook": 2,
  "firstName": "First Name 7",
  "lastName": "Last Name 7"
}
```
## 15 GET​/api​/v1​/Authors​/{3459876}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/3459876
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 404 Not Found
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-cbbc66c407ddd64f96e3d679d8ab1ac2-d665f6a9cd7c3f42-00"
}
```
## 16. PUT​/api/v1/Authors/{56}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/56
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 56,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Статус-код ответа: 200
- Тело ответа: 
```json
{
  "id": 56,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
## 17. PUT​/api/v1/Authors/{987333333655}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/987333333655
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 987333333655,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Статус-код ответа: 400 Bad Request
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-9b1e038de1dd914dbfa8e68b4ac3ccb6-8683d54e8fc26541-00",
  "errors": {
    "id": [
      "The value '987333333655' is not valid."
    ]
  }
}
```
## 18. DELETE​/api​/v1​/Authors​/{654}
Описание запроса:
- HTTP-метод: DELETE
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/654
- Заголовки запроса:  -H  "accept: */*"
- Тело запроса: отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: отсутствует

# Books 
## 19. GET​/api​/v1​/Books
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200
- Тело ответа (часть): 
```json
[[
  {
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-22T15:37:52.3418145+00:00"
  },
  {
    "id": 2,
    "title": "Book 2",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 200,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-21T15:37:52.3418277+00:00"
  },
  {
    "id": 3,
    "title": "Book 3",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 300,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-20T15:37:52.3418377+00:00"
  }
   ]
```

## 20. POST​/api​/v1​/Books
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
- Заголовки запроса: -H  "accept: */*" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-23T15:40:47.753Z"
}
```
- Статус-код ответа: 200 успешный
- Тело ответа:
```json
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-23T15:40:47.753Z"
}
```
## 21. POST​/api​/v1​/Books
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
- Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 33334689008,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-23T15:40:47.753Z"
}
```
- Статус-код ответа: 400 Bad Request
- Тело ответа:
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-f4e9a5875aeacd428fa94651b5bb554f-37b4f42bd14b2249-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 17."
    ]
  }
}
```
## 22. GET​/api/v1/Books/{55}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/55
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
{
  "id": 55,
  "title": "Book 55",
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "pageCount": 5500,
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "publishDate": "2023-04-29T15:50:41.976899+00:00"
}
```
## 23. GET​/api/v1/Books/{57854321}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/57854321
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 404 Not Found
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-b2a78772bfe6e84d918de16f6db14a50-6c9cb6aa7fcf0548-00"
}
```
## 24. PUT/api/v1/Books/{345}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/345
- Заголовки запроса:  -H  "accept: */*" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 345,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-23T15:55:58.391Z"
}
```
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
{
  "id": 345,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-23T15:55:58.391Z"
}
```
## 25. PUT/api/v1/Books/{475859590590504}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/475859590590504
- Заголовки запроса:  -H  "accept: */*" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 475859590590504,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-23T16:00:15.467Z"
}
```
- Статус-код ответа: 400 Bad Request
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-1da2971745b14144865e0383557420ed-a3c284d81cc41449-00",
  "errors": {
    "id": [
      "The value '475859590590504' is not valid."
    ]
  }
}
```
## 26. DELETE​/api​/v1​/Books​/{629}
Описание запроса:
- HTTP-метод: DELETE
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/629
- Заголовки запроса:  -H  "accept: */*"
- Тело запроса: отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: отсутствует

# CoverPhotos

## 27. GET/api/v1/CoverPhotos
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200
- Тело ответа (часть): 
```json
[
    {
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  },
  {
    "id": 2,
    "idBook": 2,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"
  },
  {
    "id": 3,
    "idBook": 3,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 3&w=250&h=350"
  },
  {
    "id": 4,
    "idBook": 4,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 4&w=250&h=350"
  }
   ]
```
## 28. POST​/api/v1/CoverPhotos
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
- Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 4,
  "idBook": 5,
  "url": "string"
}
```
- Статус-код ответа: 200 успешный
- Тело ответа:
```json
{
  "id": 4,
  "idBook": 5,
  "url": "string"
}
```
## 29. POST​/api/v1/CoverPhotos
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
- Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 345697523456789,
  "idBook": 5,
  "url": "string"
}
```
- Статус-код ответа: 400 Bad Request
- Тело ответа:
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-6a0c65fa629d0b47a2458391922fab2e-08ae20888d530647-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 21."
    ]
  }
}
```
## 30. GET​/api/v1/CoverPhotos/books/covers/{59}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/59
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
[
  {
    "id": 59,
    "idBook": 59,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 59&w=250&h=350"
  }
]
```
## 31. GET​/api/v1/CoverPhotos/books/covers/{8325977000}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/8325977000
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 400 Bad Request
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-f087c9ba7a7d3f4abbc7dfee07fcc132-0bb9bbab7aa07540-00",
  "errors": {
    "idBook": [
      "The value '8325977000' is not valid."
    ]
  }
}
```
## 32. GET/api/v1/CoverPhotos/{62}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/62
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
{
  "id": 62,
  "idBook": 62,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 62&w=250&h=350"
}
```

## 33. GET/api/v1/CoverPhotos/{678098763479}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/678098763479
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 400 Bad Request
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-cb8879223edaf44a932167d0e56d1dcb-6dfe632e61ca9a43-00",
  "errors": {
    "id": [
      "The value '678098763479' is not valid."
    ]
  }
}
```
## 34. PUT/api/v1/CoverPhotos/{84}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/84
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 84,
  "idBook": 0,
  "url": "string"
}
```
- Статус-код ответа:200 успешно
- Тело ответа: 
```json
{
  "id": 84,
  "idBook": 0,
  "url": "string"
}
```

## 35. PUT/api/v1/CoverPhotos/{8976532234570964}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/8976532234570964
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 8976532234570964,
  "idBook": 0,
  "url": "string"
}
```
- Статус-код ответа: 400 Bad Request
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-b293cc4f1964ba4cb7106b2243403389-e416d6e413963a46-00",
  "errors": {
    "id": [
      "The value '8976532234570964' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 22."
    ]
  }
}
```

## 36. DELETE​/api/v1/CoverPhotos/{629}
Описание запроса:
- HTTP-метод: DELETE
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/629
- Заголовки запроса:  -H  "accept: */*"
- Тело запроса: отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: отсутствует

# Users
## 37. GET/api/v1/Users
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
- Заголовки запроса: -H  "accept: text/plain; v=1.0"
- Тело запроса: Отсутствует
- Статус-код ответа: 200
- Тело ответа (часть): 
```json
[
     {
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
  },
  {
    "id": 2,
    "userName": "User 2",
    "password": "Password2"
  },
  {
    "id": 3,
    "userName": "User 3",
    "password": "Password3"
  },
  {
    "id": 4,
    "userName": "User 4",
    "password": "Password4"
  }
   ]
```

## 38. POST/api/v1/Users
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
- Заголовки запроса: -H  "accept: */*" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 39,
  "userName": "string",
  "password": "string"
}
```
- Статус-код ответа: 200 успешный
- Тело ответа:
```json
{
  "id": 39,
  "userName": "string",
  "password": "string"
}
```
## 39. POST/api/v1/Users
Описание запроса:
- HTTP-метод: POST
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
- Заголовки запроса: -H  "accept: */*" -H  "Content-Type: application/json; v=1.0"
- Тело запроса:
```json
{
  "id": 30095498765439,
  "userName": "string",
  "password": "string"
}
```
- Статус-код ответа: 400 Ошибка запроса
- Тело ответа:
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-97daf65394a67b4498e0eab8b612ecd8-f1c433527abc584b-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 20."
    ]
  }
}
```
## 40. GET​//api/v1/Users/{88}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/88
- Заголовки запроса: -H  "accept: */*"
- Тело запроса: Отсутствует
- Статус-код ответа: 404 Not Found
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-d8986e3101ee3442a95136d49908081a-8a2295d2b252f44c-00"
}
```
## 41. GET​//api/v1/Users/{8}
Описание запроса:
- HTTP-метод: GET
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/8
- Заголовки запроса: -H  "accept: */*"
- Тело запроса: Отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: 
```json
{
  "id": 8,
  "userName": "User 8",
  "password": "Password8"
}
```
## 42. PUT​//api/v1/Users/{42}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/42
- Заголовки запроса:  -H  "accept: */*" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 42,
  "userName": "string",
  "password": "string"
}
```
- Статус-код ответа: 200
- Тело ответа: 
```json
{
  "id": 42,
  "userName": "string",
  "password": "string"
}
```

## 43. PUT​//api/v1/Users/{547906398765432}
Описание запроса:
- HTTP-метод: PUT
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/547906398765432
- Заголовки запроса:  -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
- Тело запроса: 
 ```json
{
  "id": 547906398765432,
  "userName": "string",
  "password": "string"
}
```
- Статус-код ответа: 404 Bad Request
- Тело ответа: 
```json
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-d52c1b3a3bfaf94b8960a73ad634f203-5986595c828eca4e-00",
  "errors": {
    "id": [
      "The value '547906398765432' is not valid."
    ]
  }
}
```
## 44. DELETE​//api/v1/Users/{76}
Описание запроса:
- HTTP-метод: DELETE
- Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/33
- Заголовки запроса:  -H  "accept: */*"
- Тело запроса: отсутствует
- Статус-код ответа: 200 успешно
- Тело ответа: отсутствует