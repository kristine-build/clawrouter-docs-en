# Jimeng Video Generation

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

## Jimeng Video Generation

Jimeng official API format video generation interface.

Supports specifying operation types via the Action parameter:

* `CVSync2AsyncSubmitTask`: Submit video generation task
* `CVSync2AsyncGetResult`: Get task result

Action and Version need to be specified in the query parameters.

Endpoint POST

```
https://docs.newapi.pro/jimeng/
```

Use query parameters `Action` and `Version`. Example request path:

```
/jimeng/?Action=CVSync2AsyncSubmitTask&Version=string
```

Authorization

{% hint style="info" %}
BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`

In: `header`
{% endhint %}

Query Parameters

* Action\* (string) — API 操作类型\
  Value in `"CVSync2AsyncSubmitTask" | "CVSync2AsyncGetResult"`
* Version\* (string) — API 版本

Request Body (application/json)

* req\_key? (string) — 请求类型标识
* prompt? (string) — 文本描述
* binary\_data\_base64? (array) — Base64 编码的图片数据

Response Body

200 application/json Example:

```
{
  "code": 0,
  "message": "string",
  "data": {}
}
```

400 application/json Example:

```
{
  "error": {
    "message": "string",
    "type": "string",
    "param": "string",
    "code": "string"
  }
}
```

cURL example

```bash
curl -X POST "https://docs.newapi.pro/jimeng/?Action=CVSync2AsyncSubmitTask&Version=string" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{}'
```

Last updated on 3/1/2026

Docs home: https://docs.newapi.pro
