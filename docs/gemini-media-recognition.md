# Gemini Media Recognition

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — ChatGemini

## Gemini Media Recognition

Gemini Image, PDF, Audio, Video Recognition Request

⚠️ Note: Only supports uploading images, PDFs, audio, and video via inlineData in base64 format. fileData.fileUri or File API are not supported.

https://docs.newapi.pro

POST `/v1beta/models/{model}:generateContent`

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

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta-391536411#authorization)

### Path Parameters

model (string) — 模型名称

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta-391536411#path-parameters)

### Request Body

Content-Type: application/json

* contents? array
*   tools? array

    (Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta-391536411#request-body)

    ### Response Body

    #### 200 — application/json

    Example response:

    ```
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

    (Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta-391536411#response-body)

    ### Examples

    cURL

    ```
    curl -X POST "https://docs.newapi.pro/v1beta/models/string:generateContent" \
      -H "Authorization: Bearer " \
      -H "Content-Type: application/json" \
      -d '{}'
    ```

    JavaScript

    (Example omitted in source; preserve heading placeholder if needed.)

    Go

    (Example omitted in source; preserve heading placeholder if needed.)

    Python

    (Example omitted in source; preserve heading placeholder if needed.)

    Java

    (Example omitted in source; preserve heading placeholder if needed.)

    C#

    (Example omitted in source; preserve heading placeholder if needed.)

    Last updated on 3/1/2026

    Links referenced in this page:

    * User Guide: https://docs.newapi.pro/en/docs
    * Installation: https://docs.newapi.pro/en/docs/installation
    * API Reference: https://docs.newapi.pro/en/docs/api
    * AI Applications: https://docs.newapi.pro/en/docs/apps
    * Skills: https://docs.newapi.pro/en/docs/skills
    * Help & Support: https://docs.newapi.pro/en/docs/support
    * Business Cooperation: https://docs.newapi.pro/en/docs/business

    Additional references:

    * Path/Authorization/Request/Response docs: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta-391536411#authorization
    * Main Gemini doc: https://docs.newapi.pro/en/docs/api/ai-model/chat/gemini/geminirelayv1beta-391536411

    (End of page)
* systemInstruction? object
* safetySettings? array
* generationConfig? object
