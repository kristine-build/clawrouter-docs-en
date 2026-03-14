# Cancel Fine-tuning Task (Unimplemented)

{% hint style="warning" %}
This interface is not yet implemented
{% endhint %}

POST /v1/fine-tunes/{fine\_tune\_id}/cancel

Endpoint URL:

```
https://docs.newapi.pro/v1/fine-tunes/{fine_tune_id}/cancel
```

Request example (cURL):

```
curl -X POST "https://docs.newapi.pro/v1/fine-tunes/string/cancel" \
  -H "Authorization: Bearer "
```

Authorization

BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: header

Path Parameters

* fine\_tune\_id\* (string)

Response Body

### 501 application/json

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

Last updated on 3/1/2026

https://docs.newapi.pro
