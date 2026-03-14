# Text-to-Speech

AI Model API — Audio (OpenAI)

## Text-to-Speech

Converts text into audio.

Endpoint POST https://docs.newapi.pro/v1/audio/speech

### Authorization

BearerAuth

Authorization header:\
Authorization: Bearer

使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`

In: header

### Request Body

Content-Type: application/json

* model\* (string)
* input\* (string) — 要转换的文本\
  Length: length <= 4096
* voice\* (string) — Value in `"alloy" | "echo" | "fable" | "onyx" | "nova" | "shimmer"`
* response\_format? (string) — Default: `"mp3"`\
  Value in `"mp3" | "opus" | "aac" | "flac" | "wav" | "pcm"`
* speed? (number) — Default: `1`\
  Range: `0.25 <= value <= 4`

### Response Body

200 audio/mpeg

Sample response:

```
"string"
```

### Examples

{% tabs %}
{% tab title="cURL" %}
```
curl -X POST "https://docs.newapi.pro/v1/audio/speech" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "model": "tts-1",
    "input": "string",
    "voice": "alloy"
  }'
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
// JavaScript example
// (Original docs included a JavaScript example)
```
{% endtab %}

{% tab title="Go" %}
```go
// Go example
// (Original docs included a Go example)
```
{% endtab %}

{% tab title="Python" %}
```python
# Python example
# (Original docs included a Python example)
```
{% endtab %}

{% tab title="Java" %}
```java
// Java example
// (Original docs included a Java example)
```
{% endtab %}

{% tab title="C#" %}
```csharp
// C# example
// (Original docs included a C# example)
```
{% endtab %}
{% endtabs %}

Last updated on 3/1/2026

Related links:

* Documentation (renewed): https://doc.newapi.pro
* Old docs: https://doc.newapi.pro
* User Guide: https://docs.newapi.pro/en/docs
* Installation: https://docs.newapi.pro/en/docs/installation
* API Reference: https://docs.newapi.pro/en/docs/api
* AI Applications: https://docs.newapi.pro/en/docs/apps
* Skills: https://docs.newapi.pro/en/docs/skills
* Help & Support: https://docs.newapi.pro/en/docs/support
* Business Cooperation: https://docs.newapi.pro/en/docs/business
* Previous page: https://docs.newapi.pro/en/docs/api/ai-model/audio/geminirelayv1beta-383836364
* Next page: https://docs.newapi.pro/en/docs/api/ai-model/audio/openai/createtranscription
