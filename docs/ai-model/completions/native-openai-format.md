# Native OpenAI Format

Native OpenAI Format

Create text completions based on a given prompt.

Endpoint POST https://docs.newapi.pro/v1/completions

Authorization

See: https://docs.newapi.pro/en/docs/api/ai-model/completions/createcompletion#authorization

BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: header

Request Body

Content-Type: application/json — see: https://docs.newapi.pro/en/docs/api/ai-model/completions/createcompletion#request-body

* model\* string
* prompt\* string | array
* max\_tokens? integer
* temperature? number
* top\_p? number
* n? integer
* stream? boolean
* stop? string | array
* suffix? string
* echo? boolean

Response Body

200 application/json — see: https://docs.newapi.pro/en/docs/api/ai-model/completions/createcompletion#response-body

Example request (cURL)

{% code title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/v1/completions" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "model": "string",
    "prompt": "string"
  }'
```
{% endcode %}

Example 200 response

```json
{
  "id": "string",
  "object": "text_completion",
  "created": 0,
  "model": "string",
  "choices": [
    {
      "text": "string",
      "index": 0,
      "finish_reason": "string"
    }
  ],
  "usage": {
    "prompt_tokens": 0,
    "completion_tokens": 0,
    "total_tokens": 0,
    "prompt_tokens_details": {
      "cached_tokens": 0,
      "text_tokens": 0,
      "audio_tokens": 0,
      "image_tokens": 0
    },
    "completion_tokens_details": {
      "text_tokens": 0,
      "audio_tokens": 0,
      "reasoning_tokens": 0
    }
  }
}
```

Last updated on 3/1/2026
