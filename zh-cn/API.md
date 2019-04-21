# API

## 定义
**IPN - 推送通知**  
类似手机的App可以给你发送推送通知，
我们也可以发送事件推送通知至你的服务器。
一些规则将在后文详细阐述。

**令牌**   
我们采用令牌来区分用户。每一个用户都有一个独立的令牌。

**错误枚举**  
TODO

## 用户 API
**获取用户令牌**  
POST [/userLogin]()  
请求:
```JSON
{
  "userParam": "blablabla@test.com",
  "password": "myHugeSecret"
}
```
**userParam** 是用户邮箱/用户名  
**password** 是用户密码

返回数据:
```json
{
  "info": "a2fd23mw4-1",
  "success": 1
}
```
**info** 是用户令牌或者错误信息  
**success** 体现info是否为用户令牌

## 爬虫任务 API
TODO

## 语义分析 API
TODO