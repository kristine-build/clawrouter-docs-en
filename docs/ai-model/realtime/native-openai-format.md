# Native OpenAI Format

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — Realtime

## Native OpenAI Format

Establish a WebSocket connection for real-time conversations.

Note: This is a WebSocket endpoint and requires a WebSocket protocol connection.

Connection URL example: `wss://api.example.com/v1/realtime?model=gpt-4o-realtime`

https://docs.newapi.pro

GET

`/v1/realtime`

Send

Authorization

### Authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/realtime/createrealtimesession#authorization)

### Query Parameters

model?string

要使用的模型

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/realtime/createrealtimesession#query-parameters)

### Response Body

#### 101

Empty

#### 400 application/json

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

Code samples

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X GET "https://docs.newapi.pro/v1/realtime" \
  -H "Authorization: Bearer "
```
{% endtab %}
{% endtabs %}

Last updated on 3/1/2026
