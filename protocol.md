## Remind
## 获取提醒的相关信息
### [Name]
getRemind
### [Request]
```json
{
     "body":{}
}
```
### [Response]
```json
{
    "body":{
         "code":0,
         "msg":"ok",
         "data":{"on": 1, "pd": 30}
    }
}
```

## 设置提醒相关信息
### [Name]
setRemind
### [Request]
```json
{
    "body":{
        "data":{"on": 1, "pd": 30}
    }
}
```

### [Response]
```json
{
    "body":{
        "code":0,
        "msg":"ok",
    }
}
```
## report提醒信息变化
### [Name]
onRemind
### [Report]
```json
{
      "body":{
          "data":{"on": 1, "pd": 30}
      }
}
```
### [Parameters]
* Remind 结构说明：
  *  on:integer, 1、提醒开；0、提醒关。可缺省。
  *  pd:int
  * 具体的json schema 可参考：<br/>
    http://rcp-schema.ecouser.net/Data/Config/Remind.json