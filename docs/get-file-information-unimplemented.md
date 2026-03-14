# Get File Information (Unimplemented)

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — Unimplemented Files

## Get File Information (Unimplemented)

This interface is not yet implemented.

Base URL https://docs.newapi.pro

Endpoint GET /`v1`/`files`/`{file_id}`

Authorization BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: header

Path Parameters

* file\_id\* string

Response Body

#### 501 application/json

Example curl

```
curl -X GET "https://docs.newapi.pro/v1/files/string" \
  -H "Authorization: Bearer "
```

Response (501)

```json
{
  "error": {
    "message": "string",
    "type": "string",
    "param": "string",
    "code": "string"
  }
}
```

Related links

* https://docs.newapi.pro/en/docs/api/ai-model/unimplemented/files/listfiles
* https://docs.newapi.pro/en/docs/api/ai-model/unimplemented/fine-tuning/cancelfinetune

Last updated on 3/1/2026
