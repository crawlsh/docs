# API
We have only 3 but enough APIs!

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
APIs that deal with user affairs
#### Get User Token  
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
  "info": "dda7f8f6ccf95166ce90f530d656242409f9bc19",
  "success": 1
}
```
**info** is user token/fail message  
**success** is whether login is success

## Job API
APIs that deal with crawl tasks
#### Get All Jobs
GET [/getAllJobs]()  
Request:  
```
{
  "token": dda7f8f6ccf95166ce90f530d656242409f9bc19"
}
```
**token** is user token

Response:
```json
[{
    "jobToken": "05d08be94045823eef0c557159a3d4da94cef988",
    "progress": [100, "Done"],
    "content": "https://google.com/",
    "time": "1559109874",
    "_type": "CRAWL"
}]
```
**jobToken** is job token  
**progress** is [progress of job, notices]  
**content** is name of the job   
**time** is the time of the start of the job

#### Get Detail of a Job
GET [/getResult]()  
Request:  
```
{
  "jobToken": 05d08be94045823eef0c557159a3d4da94cef988"
}
```
**jobToken** is job token

Response:
```json
{
  "info": [
    {
      
    }
  ], 
  "success": 1
}
```
**jobToken** is job token  
**progress** is [progress of job, notices]  
**content** is name of the job   
**time** is the time of the start of the job

## NLP API
TODO
