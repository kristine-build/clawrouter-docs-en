# Native Gemini Format

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

## AI Model API — Models List

## Native Gemini Format

Returns a list of available models in Gemini API format.

Endpoint GET `/`v1beta`/models`

Request example

```
curl -X GET "https://loading/v1beta/models"
```

Authorization

See: https://docs.newapi.pro/en/docs/api/ai-model/models/list/listmodelsgemini#authorization

BearerAuth

Authorization header format:

```
Authorization: Bearer <token>
```

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

Response Body

#### 200 application/json

Example response:

```json
{
  "models": [
    {
      "name": "models/gemini-pro",
      "version": "string",
      "displayName": "string",
      "description": "string",
      "inputTokenLimit": 0,
      "outputTokenLimit": 0,
      "supportedGenerationMethods": [
        "string"
      ]
    }
  ]
}
```

Related pages

* Native OpenAI Format (GET): https://docs.newapi.pro/en/docs/api/ai-model/models/list/listmodels
* Native OpenAI Format (POST): https://docs.newapi.pro/en/docs/api/ai-model/moderations/createmoderation
