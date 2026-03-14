# Native Gemini Format

Native Gemini Format

Gemini audio generation API. Models such as gemini-2.5-flash-preview-tts can be used.

https://docs.newapi.pro

POST `/v1beta/models/{model}:generateContent`

Authorization

* BearerAuth
* Header: Authorization: Bearer
* 使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`
* In: `header`

Path Parameters

* model\* string — 模型名称

Request Body (application/json)

*   contents\* array

    Example cURL request

    ```bash
    curl -X POST "https://docs.newapi.pro/v1beta/models/string:generateContent" \
      -H "Authorization: Bearer " \
      -H "Content-Type: application/json" \
      -d '{
        "contents": [\
          {}\
        ],
        "generationConfig": {
          "responseModalities": [\
            "string"\
          ],
          "speechConfig": {
            "voiceConfig": {
              "prebuiltVoiceConfig": {
                "voiceName": "string"
              }
            }
          }
        }
      }'
    ```

    Example 200 response (application/json)

    ```json
    {
      "candidates": [\
        {\
          "content": {\
            "role": "string",\
            "parts": [\
              {}\
            ]\
          },\
          "finishReason": "string",\
          "safetyRatings": [\
            {}\
          ]\
        }\
      ],
      "usageMetadata": {
        "promptTokenCount": 0,
        "candidatesTokenCount": 0,
        "totalTokenCount": 0
      }
    }
    ```

    Last updated on 3/1/2026

    Reference

    * Authorization: https://docs.newapi.pro/en/docs/api/ai-model/audio/geminirelayv1beta-383836364#authorization
    * Path Parameters: https://docs.newapi.pro/en/docs/api/ai-model/audio/geminirelayv1beta-383836364#path-parameters
    * Request Body: https://docs.newapi.pro/en/docs/api/ai-model/audio/geminirelayv1beta-383836364#request-body
    * Response Body: https://docs.newapi.pro/en/docs/api/ai-model/audio/geminirelayv1beta-383836364#response-body

    (For other language examples shown in the original docs: cURL, JavaScript, Go, Python, Java, C# — see the main documentation.)
* generationConfig\* object
