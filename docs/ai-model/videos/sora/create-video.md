# Create Video

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

AI Model APIVideosSora

## Create Video

OpenAI-compatible video generation API.

Reference documentation: https://platform.openai.com/docs/api-reference/videos/create

https://docs.newapi.pro

POST

`/`v1`/`videos\`

Send

### Authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### Request Body

Content type: multipart/form-data

* model?string\
  模型/风格 ID
* prompt?string\
  文本描述提示词
* image?string\
  图片输入 (URL 或 Base64)
* duration?number\
  视频时长（秒）
* width?integer\
  视频宽度
* height?integer\
  视频高度
* fps?integer\
  视频帧率
* seed?integer\
  随机种子
* n?integer\
  生成视频数量
* response\_format?string\
  响应格式
* user?string\
  用户标识
* metadata?object\
  扩展参数 (如 negative\_prompt, style, quality\_level 等)

### Response Body

#### 200 application/json

```json
{
  "id": "string",
  "object": "string",
  "model": "string",
  "status": "string",
  "progress": 0,
  "created_at": 0,
  "seconds": "string",
  "completed_at": 0,
  "expires_at": 0,
  "size": "string",
  "error": {
    "message": "string",
    "code": "string"
  },
  "metadata": {}
}
```

#### 400 application/json

```json
{
  "error": {
    "message": "string",
    "type": "string",
    "param": "string",
    "code": "string"
  }
}
```

### Example

{% tabs %}
{% tab title="cURL" %}
```
curl -X POST "https://docs.newapi.pro/v1/videos" \
  -H "Authorization: Bearer "
```
{% endtab %}
{% endtabs %}

Languages referenced: JavaScript, Go, Python, Java, C#

Last updated on 3/1/2026

Reference: https://docs.newapi.pro

Reference documentation: [https://platform.openai.com/docs/api-reference/videos/create](https://platform.openai.com/docs/api-reference/videos/create)
