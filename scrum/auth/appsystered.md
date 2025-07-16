```sh

### Find All Users
GET https://appsystered.com/api/users/findAll
Authorization: Bearer eyJhbGciOiJIUzI1N...


### Register
POST https://appsystered.com/api/auth/register
Content-Type: application/json

{
    "name": "user 2",
    "email": "user2@gmail.com",
    "password": "password123"
}


### Login
POST https://appsystered.com/api/auth/login
Content-Type: application/json

{
    "email": "user3@gmail.com",
    "password": "password123"
}


### Delete
DELETE https://appsystered.com/api/users/remove/68782b97b1ba8015d2a9b6fd
Authorization: Bearer eyJhbGciOiJIUzI1N...
```
