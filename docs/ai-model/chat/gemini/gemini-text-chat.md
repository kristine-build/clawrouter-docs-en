# Gemini Text Chat

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

AI Model API — ChatGemini

## Gemini Text Chat

Copy MarkdownOpen

Proxy Gemini API requests. Path format: `/v1beta/models/{model_name}:{action}`

For example:

* `/v1beta/models/gemini-2.5-pro:generateContent`
* `/v1beta/models/gemini-2.5-pro:streamGenerateContent?alt=sse`

https://docs.newapi.pro

POST

`/`v1beta`/`models`/`{model}:generateContent\`

Send

Authorization

Path

Body

### Authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta#authorization)

### Path Parameters

model — string

模型名称

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta#path-parameters)

### Request Body

Content-Type: application/json

* contents? — array
*   tools? — array

    (Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta#request-body)

    ### Response Body

    #### 200 application/json

    (Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta#response-body)

    ### Examples

    cURL

    ```bash
    curl -X POST "https://docs.newapi.pro/v1beta/models/string:generateContent" \
      -H "Authorization: Bearer " \
      -H "Content-Type: application/json" \
      -d '{}'
    ```

    Example 200 response

    ```json
    {
      "candidates": [
        {
          "content": {
            "role": "string",
            "parts": [
              {}
            ]
          },
          "finishReason": "string",
          "safetyRatings": [
            {}
          ]
        }
      ],
      "usageMetadata": {
        "promptTokenCount": 0,
        "candidatesTokenCount": 0,
        "totalTokenCount": 0
      }
    }
    ```

    How is this guide?

    GoodBad

    Last updated on 3/1/2026

    [Gemini Media RecognitionPOST](../../../gemini-media-recognition.md) — [ChatCompletions FormatPOST](../openai/chatcompletions-format.md)
* systemInstruction? — object
* safetySettings? — array
* generationConfig? — object
