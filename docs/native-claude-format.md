# Native Claude Format

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — Chat

Native Claude Format

Requests in Anthropic Claude Messages API format. Requires `anthropic-version` in the request header.

Endpoint POST /v1/messages

Full docs: https://docs.newapi.pro

Authorization

BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: header

Header Parameters

* anthropic-version _string_\
  Anthropic API 版本
* x-api-key ?string\
  Anthropic API Key (可选，也可使用 Bearer Token)

Request Body (application/json)

* model _string_
* messages _arraysystem ?string|arraymax\_tokens integer_\
  &#xNAN;_&#x52;ange `1 <= value`temperature ?number_\
  &#xNAN;_&#x52;ange `0 <= value <= 1`top\_p ?numbertop\_k ?integerstream ?booleanstop\_sequences ?arraytools ?arraytool\_choice ?objectthinking ?objectmetadata ?objectResponse Body200 application/jsoncUR&#x4C;_&#x63;url -X POST "https://docs.newapi.pro/v1/messages" \  -H "anthropic-version: 2023-06-01" \  -H "Authorization: Bearer " \  -H "Content-Type: application/json" \  -d '{    "model": "claude-3-opus-20240229",    "messages": \[\      {\        "role": "user",\        "content": "string"\      }\    ],    "max\_tokens": 1  }'_Example 200 response_{  "id": "string",  "type": "message",  "role": "assistant",  "content": \[\    {\      "type": "string",\      "text": "string"\    }\  ],  "model": "string",  "stop\_reason": "end\_turn",  "usage": {    "input\_tokens": 0,    "output\_tokens": 0,    "cache\_creation\_input\_tokens": 0,    "cache\_read\_input\_tokens": 0  \}}_Additional links referenced in this pageAuthorization: https://docs.newapi.pro/en/docs/api/ai-model/chat/createmessage#authorizationHeader Parameters: https://docs.newapi.pro/en/docs/api/ai-model/chat/createmessage#header-parametersRequest Body: https://docs.newapi.pro/en/docs/api/ai-model/chat/createmessage#request-bodyResponse Body: https://docs.newapi.pro/en/docs/api/ai-model/chat/createmessage#response-body_
