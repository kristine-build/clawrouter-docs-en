# Native OpenAI Format

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — Embeddings

## Native OpenAI Format

Convert text to vector embeddings

Endpoint POST https://docs.newapi.pro/v1/embeddings

Authorization BearerAuth

Authorization Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: header

Request Body (application/json)

* model\* string
* input\* string | array\
  要嵌入的文本
* encoding\_format? string\
  Default: `"float"`\
  Value in `"float" | "base64"`
* dimensions? integer\
  输出向量维度

Response Body

#### 200 application/json

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/v1/embeddings" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "model": "text-embedding-ada-002",
    "input": "string"
  }'
```
{% endtab %}
{% endtabs %}

Example 200 response:

```json
{
  "object": "list",
  "data": [
    {
      "object": "embedding",
      "index": 0,
      "embedding": [
        0
      ]
    }
  ],
  "model": "string",
  "usage": {
    "prompt_tokens": 0,
    "total_tokens": 0
  }
}
```

Last updated on 3/1/2026
