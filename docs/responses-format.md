# Responses Format

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — ChatOpenai

## Responses Format

Copy MarkdownOpen

OpenAI Responses API, used to create model responses. Supports multi-turn conversations, tool calling, reasoning, and other features.

https://docs.newapi.pro

POST

```
/`v1`/responses
```

Send

Authorization

Body

### Authorization

https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createresponse#authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。 格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### Request Body

https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createresponse#request-body

Content type: application/json

* model\* string
* input? string|array\
  输入内容，可以是字符串或消息数组
* tool\_choice? string|object
* reasoning? object
* previous\_response\_id? string
* truncation? string\
  Value in `"auto" | "disabled"`
*   tools? array

    #### Response Body

    https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createresponse#response-body

    **200 application/json**

    cURL

    ```bash
    curl -X POST "https://docs.newapi.pro/v1/responses" \
      -H "Authorization: Bearer " \
      -H "Content-Type: application/json" \
      -d '{
        "model": "string"
      }'
    ```

    Example 200 response:

    ```json
    {
      "id": "string",
      "object": "response",
      "created_at": 0,
      "status": "completed",
      "model": "string",
      "output": [
        {
          "type": "string",
          "id": "string",
          "status": "string",
          "role": "string",
          "content": [
            {
              "type": "string",
              "text": "string"
            }
          ]
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

    For full documentation visit: https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createresponse
* stream? boolean
* top\_p? number
* temperature? number
* max\_output\_tokens? integer
* instructions? string
