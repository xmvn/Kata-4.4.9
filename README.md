# Kata-4.4.9

## 1. Регистрация 

URL: https://blog.kata.academy/api/users/  
Method: POST

Body:
```json
{
    "user":{
        "username": "sasai",
        "email": "tensai.z@yandex.ru",
        "password": "password"
    }
}
```
Response: 

```json
{
    "user": {
        "username": "sasai",
        "email": "tensai.z@yandex.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1MDk3NDc0YzMxZGUxMWIwMGJjZDc2NiIsInVzZXJuYW1lIjoic2FzYWkiLCJleHAiOjE3MDAzMDI0NTIsImlhdCI6MTY5NTExODQ1Mn0.D9FR7QETnN9fleIDQN7AR2Orp2xkEDhIs3A1A-KE528"
    }
}
```

## 2. Аутентификация


URL: https://blog.kata.academy/api/users/login  
Method: POST

Body:
```json
{
  "user": {
  "email": "tensai.z@yandex.ru",
  "password": "password"
}
}
```

Response:
```json
{
    "user": {
        "username": "sasai",
        "email": "tensai.z@yandex.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1MDk3NDc0YzMxZGUxMWIwMGJjZDc2NiIsInVzZXJuYW1lIjoic2FzYWkiLCJleHAiOjE3MDAzMDI5NjUsImlhdCI6MTY5NTExODk2NX0.xwjd9aVw5TTEtrKSK2ZCppo0a-L4ATAPXKJ9egngPGg"
    }
}
```

## 3. Получение данных пользователя


URL: https://blog.kata.academy/api/user  
Method: GET

Headers:
```
Key: Content-Type, Value: application/json
Key: Authorization, Value: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1MDk3NDc0YzMxZGUxMWIwMGJjZDc2NiIsInVzZXJuYW1lIjoic2FzYWkiLCJleHAiOjE3MDAzMDI0NTIsImlhdCI6MTY5NTExODQ1Mn0.D9FR7QETnN9fleIDQN7AR2Orp2xkEDhIs3A1A-KE528
```

Response:
```json
{
    "user": {
        "username": "sasai",
        "email": "tensai.z@yandex.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1MDk3NDc0YzMxZGUxMWIwMGJjZDc2NiIsInVzZXJuYW1lIjoic2FzYWkiLCJleHAiOjE3MDAzMDMyNTgsImlhdCI6MTY5NTExOTI1OH0.VhepAmAcgdq8oLjer7lZtVD_kYZC5Fh5x92Gs84F2To"
    }
}
```
