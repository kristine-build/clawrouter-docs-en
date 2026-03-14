# OpenAI Chat Format

For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

AI Model API › Images › Gemini

## OpenAI Chat Format

Gemini Image Generation

https://docs.newapi.pro

POST

`/`v1`/`chat`/`completions\`

Send

Authorization

Body

### Authorization

[Authorization](openai-chat-format.md#authorization)

BearerAuth

`Authorization: Bearer <token>`

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### Request Body

[Request Body](openai-chat-format.md#request-body)

Content type: `application/json`

Required fields:

* model \*string
* stream \*boolean
* messages \*array
*   contents \*array

    Optional:

    * extra\_body? object

    ### Response Body

    [Response Body](openai-chat-format.md#response-body)

    #### 200 application/json

    ```json
    {
      "id": "string",
      "model": "string",
      "object": "string",
      "created": 0,
      "choices": [
        {
          "index": 0,
          "message": {
            "role": "string",
            "content": "string"
          },
          "finish_reason": "string"
        }
      ],
      "usage": {
        "prompt_tokens": 0,
        "completion_tokens": 0,
        "total_tokens": 0
      }
    }
    ```

    How is this guide?

    Good Bad

    Last updated on 3/1/2026
