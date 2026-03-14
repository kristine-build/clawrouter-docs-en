# Native OpenAI Format

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

## AI Model APIModerations

Native OpenAI Format

Check if text content violates usage policy

https://docs.newapi.pro

POST `/`v1`/`moderations\`

Send

Authorization

Body

### Authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### Request Body

application/json

input\*string|array

model?string

### Response Body

#### 200 application/json

cURL

```
curl -X POST "https://docs.newapi.pro/v1/moderations" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "input": "string"
  }'
```

Response (200)

```
{
  "id": "string",
  "model": "string",
  "results": [\
    {\
      "flagged": true,\
      "categories": {},\
      "category_scores": {}\
    }\
  ]
}
```

How is this guide?

GoodBad

Last updated on 3/1/2026
