# Edit Image

百炼qwen-image series image editing

Endpoint POST `/v1/images/edits`

Base URL: https://docs.newapi.pro

Authorization Bearer Auth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: header

Request Body (application/json)

* model\* string
* input\* object
* parameters? object

Response Body

200 — application/json

Example request (cURL)

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/v1/images/edits" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "model": "string",
    "input": {
      "messages": [\
        {}\
      ]
    }
  }'
```
{% endtab %}
{% endtabs %}

Example 200 response

```json
{
  "created": 0,
  "data": [\
    {\
      "url": "string",\
      "b64_json": "string",\
      "revised_prompt": "string"\
    }\
  ]
}
```

Last updated on 3/1/2026
