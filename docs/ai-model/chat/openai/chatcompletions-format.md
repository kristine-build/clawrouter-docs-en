# ChatCompletions Format

## AI Model API — Chat (OpenAI)

## ChatCompletions Format

Creates model responses based on chat history. Supports streaming and non-streaming responses.

Compatible with OpenAI Chat Completions API.

https://docs.newapi.pro

POST

```
/`v1`/`chat`/`completions
```

Send

Authorization

Body

### Authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createchatcompletion#authorization)

### Request Body

Content type: application/json

(Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createchatcompletion#request-body)

* model\* (string)\
  模型 ID
* messages\* (array)\
  对话消息列表temperature? (number)\
  采样温度\
  Default `1`\
  Range `0 <= value <= 2`top\_p? (number)\
  核采样参数\
  Default `1`\
  Range `0 <= value <= 1`n? (integer)\
  生成数量\
  Default `1`\
  Range `1 <= value`stream? (boolean)\
  是否流式响应\
  Default `false`stream\_options? (object)stop? (string | array)\
  停止序列max\_tokens? (integer)\
  最大生成 Token 数max\_completion\_tokens? (integer)\
  最大补全 Token 数presence\_penalty? (number)\
  Default `0`\
  Range `-2 <= value <= 2`frequency\_penalty? (number)\
  Default `0`\
  Range `-2 <= value <= 2`logit\_bias? (object)user? (string)tools? (array)tool\_choice? (string | object)response\_format? (object)seed? (integer)reasoning\_effort? (string)\
  推理强度 (用于支持推理的模型)\
  Value in `"low" | "medium" | "high"`modalities? (array)audio? (object)Response Body(Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createchatcompletion#response-body)200 application/json400 application/json429 application/jsonExamplescurl -X POST "https://docs.newapi.pro/v1/chat/completions" \  -H "Authorization: Bearer " \  -H "Content-Type: application/json" \  -d '{    "model": "gpt-4",    "messages": \[\      {\        "role": "system",\        "content": "string"\      }\    ]  }'curl -X POST "https://docs.newapi.pro/v1/chat/completions" \  -H "Authorization: Bearer " \  -H "Content-Type: application/json" \  -d '{    "model": "gpt-4",    "messages": \[\      {\        "role": "system",\        "content": "string"\      }\    ]  }'curl -X POST "https://docs.newapi.pro/v1/chat/completions" \  -H "Authorization: Bearer " \  -H "Content-Type: application/json" \  -d '{    "model": "gpt-4",    "messages": \[\      {\        "role": "system",\        "content": "string"\      }\    ]  }'curl -X POST "https://docs.newapi.pro/v1/chat/completions" \  -H "Authorization: Bearer " \  -H "Content-Type: application/json" \  -d '{    "model": "gpt-4",    "messages": \[\      {\        "role": "system",\        "content": "string"\      }\    ]  }'curl -X POST "https://docs.newapi.pro/v1/chat/completions" \  -H "Authorization: Bearer " \  -H "Content-Type: application/json" \  -d '{    "model": "gpt-4",    "messages": \[\      {\        "role": "system",\        "content": "string"\      }\    ]  }'curl -X POST "https://docs.newapi.pro/v1/chat/completions" \  -H "Authorization: Bearer " \  -H "Content-Type: application/json" \  -d '{    "model": "gpt-4",    "messages": \[\      {\        "role": "system",\        "content": "string"\      }\    ]  }'Sample 200 Response{  "id": "string",  "object": "chat.completion",  "created": 0,  "model": "string",  "choices": \[\    {\      "index": 0,\      "message": {\        "role": "system",\        "content": "string",\        "name": "string",\        "tool\_calls": \[\          {\            "id": "string",\            "type": "function",\            "function": {\              "name": "string",\              "arguments": "string"\            }\          }\        ],\        "tool\_call\_id": "string",\        "reasoning\_content": "string"\      },\      "finish\_reason": "stop"\    }\  ],  "usage": {    "prompt\_tokens": 0,    "completion\_tokens": 0,    "total\_tokens": 0,    "prompt\_tokens\_details": {      "cached\_tokens": 0,      "text\_tokens": 0,      "audio\_tokens": 0,      "image\_tokens": 0    },    "completion\_tokens\_details": {      "text\_tokens": 0,      "audio\_tokens": 0,      "reasoning\_tokens": 0    }  },  "system\_fingerprint": "string"}Sample Error Response{  "error": {    "message": "string",    "type": "string",    "param": "string",    "code": "string"  \}}Last updated on 3/1/2026Reference: https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/createchatcompletion
