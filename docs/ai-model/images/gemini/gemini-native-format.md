# Gemini Native Format

Gemini Image Generation

https://docs.newapi.pro

POST `/v1beta/models/{model}:generateContent/`

Send

## Authorization

BearerAuth

Authorization `Authorization: Bearer <token>`

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

(See: https://docs.newapi.pro/en/docs/api/ai-model/images/gemini/geminirelayv1beta-383837589#authorization)

## Path Parameters

* model (string) — 模型名称

(See: https://docs.newapi.pro/en/docs/api/ai-model/images/gemini/geminirelayv1beta-383837589#path-parameters)

## Request Body

Content-Type: application/json

*   contents\* — array

    (See: https://docs.newapi.pro/en/docs/api/ai-model/images/gemini/geminirelayv1beta-383837589#request-body)

    ### Response Body

    #### 200 — application/json

    (See: https://docs.newapi.pro/en/docs/api/ai-model/images/gemini/geminirelayv1beta-383837589#response-body)

    cURL

    ```bash
    curl -X POST "https://docs.newapi.pro/v1beta/models/string:generateContent/" \
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
          "imageConfig": {
            "aspectRatio": "string",
            "imageSize": "string"
          }
        }
      }'
    ```

    Example 200 response:

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

    Related links:

    * Documentation renewed: https://doc.newapi.pro/
    * Older docs and sections:
      * User Guide: https://docs.newapi.pro/en/docs
      * Installation: https://docs.newapi.pro/en/docs/installation
      * API Reference: https://docs.newapi.pro/en/docs/api
      * AI Applications: https://docs.newapi.pro/en/docs/apps
      * Skills: https://docs.newapi.pro/en/docs/skills
      * Help & Support: https://docs.newapi.pro/en/docs/support
      * Business Cooperation: https://docs.newapi.pro/en/docs/business

    (Original source: https://docs.newapi.pro)
* generationConfig\* — object
