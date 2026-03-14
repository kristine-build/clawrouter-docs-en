# Document Reranking

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

AI Model: APIRerank

## Document Reranking

Rerank document list by relevance based on query

Endpoint https://docs.newapi.pro

POST `/v1/rerank`

### Authorization

BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: header

### Request Body

Content-Type: application/json

* model\* string
* query\* string — 查询文本
* documents\* array\<string | object> — 要重排序的文档列表
* top\_n? integer — 返回前 N 个结果
* return\_documents? boolean — Default `false`

### Example: cURL

```
curl -X POST "https://docs.newapi.pro/v1/rerank" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "model": "rerank-english-v2.0",
    "query": "string",
    "documents": [
      "string"
    ]
  }'
```

### Response Body

200 application/json

Example response:

```
{
  "id": "string",
  "results": [
    {
      "index": 0,
      "relevance_score": 0,
      "document": {}
    }
  ],
  "meta": {}
}
```

Last updated on 3/1/2026
