# API
We provide versatile SDKs for linking your system to 
our system.

## Definition
**IPN - Instant Push Notification**  
Like Apps could send notification to your phone, we
could also send notification to your server. A few 
conventions would be discussed later.

**Token**   
We use token to identify user. Each user gets an unique
token. 

**Failure Enumerations**  
TODO

## User API
**Get User Token**  
POST [/userLogin]()  
Request:  
```JSON
{
  "userParam": "blablabla@test.com",
  "password": "myHugeSecret"
}
```
**userParam** is user email/username  
**password** is user password

Response:
```json
{
  "info": "a2fd23mw4-1",
  "success": 1
}
```
**info** is user token/fail message  
**success** is whether login is success

## Job API
TODO

## NLP API
TODO