# Native Gemini Format

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — Embeddings

## Native Gemini Format

Create Embeddings using a specified engine/model

Endpoint POST `/v1/engines/{model}/embeddings`

Full URL: https://docs.newapi.pro

Authorization BearerAuth

Authorization header Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`\
In: header

Path Parameters

* model (string, required)\
  模型/引擎 ID

Request Body (application/json)

* model (string, required)
* input (string | array, required)\
  要嵌入的文本
* encoding\_format (string, optional)\
  Default: `"float"`\
  Value in `"float" | "base64"`
* dimensions (integer, optional)\
  输出向量维度

Response Body

200 — application/json

Example requests

curl

```
curl -X POST "https://docs.newapi.pro/v1/engines/string/embeddings" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "model": "text-embedding-ada-002",
    "input": "string"
  }'
```

Example 200 response

```
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

Related

* Native OpenAI Format: https://docs.newapi.pro/en/docs/api/ai-model/embeddings/createembedding
* Gemini Native Format (Images): https://docs.newapi.pro/en/docs/api/ai-model/images/gemini/geminirelayv1beta-383837589
