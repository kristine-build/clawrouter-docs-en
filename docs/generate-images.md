# Generate Images

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

AI Model API Images Qwen

## Generate Images

Bailian qwen-image series image generation

POST /v1/images/generations

### Authorization

BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

(See: https://docs.newapi.pro/en/docs/api/ai-model/images/qwen/createimage#authorization)

### Request Body

Content-Type: application/json

Fields:

* model\* string
* input\* object
* parameters? object

(See: https://docs.newapi.pro/en/docs/api/ai-model/images/qwen/createimage#request-body)

### Response Body

200 — application/json

Example request (cURL):

```
curl -X POST "https://loading/v1/images/generations" \
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

Example response (200):

```
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

Links to related pages:

* Create Image (authorization & request/response details): https://docs.newapi.pro/en/docs/api/ai-model/images/qwen/createimage#authorization
* API Reference (previous example): https://docs.newapi.pro/en/docs/api/ai-model/images/openai/post-v1-images-generations
* Edit Image: https://docs.newapi.pro/en/docs/api/ai-model/images/qwen/editimage

How is this guide? Good Bad
