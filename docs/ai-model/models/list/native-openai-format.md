# Native OpenAI Format

AI Model API — Models List

## Native OpenAI Format

Get a list of currently available models.

Automatically identifies the return format based on the request headers:

* Returns Anthropic format when `x-api-key` and `anthropic-version` headers are present
* Returns Gemini format when `x-goog-api-key` header or `key` query parameter is present
* Returns OpenAI format in other cases

Endpoint GET https://docs.newapi.pro/v1/models

Full docs: https://docs.newapi.pro

Authorization BearerAuth

Header Authorization: Bearer

使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

Query Parameters

* key? string\
  Google API Key (用于 Gemini 格式)

Header Parameters

* x-api-key? string\
  Anthropic API Key (用于 Claude 格式)
* anthropic-version? string\
  Anthropic API 版本
* x-goog-api-key? string\
  Google API Key (用于 Gemini 格式)

Response Body

* 200 — application/json
* 401 — application/json

Example request (cURL)

```bash
curl -X GET "https://loading/v1/models"
```

Example 200 response

```json
{
  "object": "list",
  "data": [
    {
      "id": "gpt-4",
      "object": "model",
      "created": 0,
      "owned_by": "openai"
    }
  ]
}
```

Example 401 error response

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

Client libraries / example languages

* cURL
* JavaScript
* Go
* Python
* Java
* C#

Related

* Documentation renewed! For old docs, visit: https://doc.newapi.pro/
* User Guide: https://docs.newapi.pro/en/docs
* Installation: https://docs.newapi.pro/en/docs/installation
* API Reference: https://docs.newapi.pro/en/docs/api
* AI Applications: https://docs.newapi.pro/en/docs/apps
* Skills: https://docs.newapi.pro/en/docs/skills
* Help & Support: https://docs.newapi.pro/en/docs/support
* Business Cooperation: https://docs.newapi.pro/en/docs/business

Last updated on 3/1/2026
