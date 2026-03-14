# Get Video Task Status

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model: APIVideosSora

## Get Video Task Status

OpenAI-compatible video task status query interface.

Returns detailed status information for video tasks.

Endpoint GET `/`v1`/`videos`/`{task\_id}\`

Base URL: https://docs.newapi.pro

### Authorization

BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### Path Parameters

* task\_id\* string — 视频任务 ID

### Response Body

#### 200 application/json

Example:

```json
{
  "id": "string",
  "object": "string",
  "model": "string",
  "status": "string",
  "progress": 0,
  "created_at": 0,
  "seconds": "string"
}
```

#### 404 application/json

Example:

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

### Examples

cURL

{% code title="cURL" %}
```bash
curl -X GET "https://docs.newapi.pro/v1/videos/string" \
  -H "Authorization: Bearer "
```
{% endcode %}

(JavaScript, Go, Python, Java, C# examples omitted in source — include platform-specific examples here if available.)

Last updated on 3/1/2026
