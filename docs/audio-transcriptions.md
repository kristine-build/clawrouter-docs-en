# Audio Transcriptions

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — Audio — Openai

## Audio Transcriptions

Convert audio to text.

Endpoint

* POST https://docs.newapi.pro/v1/audio/transcriptions

Authorization

* Type: BearerAuth
* Header: Authorization: Bearer
* Description: 使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`
* In: header

Request body (multipart/form-data)

* file\* (file) — 音频文件 (Format: binary)
* model\* (string)
* language? (string) — ISO-639-1 语言代码
* prompt? (string)
* response\_format? (string) — Default: `"json"`. Value in `"json" | "text" | "srt" | "verbose_json" | "vtt"`
* temperature? (number)
* timestamp\_granularities? (array)

Response body

200 application/json

Example response:

```
{
  "text": "string"
}
```

Example cURL

```
curl -X POST "https://docs.newapi.pro/v1/audio/transcriptions" \
  -H "Authorization: Bearer " \
  -F file="string" \
  -F model="whisper-1"
```

Last updated on 3/1/2026

Related

* Text-to-Speech: https://docs.newapi.pro/en/docs/api/ai-model/audio/openai/createspeech
* Audio Translation: https://docs.newapi.pro/en/docs/api/ai-model/audio/openai/createtranslation
