# Kling Text-to-Video

AI Model APIVideosKling

## Kling Text-to-Video

Generate videos from text descriptions using the Kling model.

Supported models: kling-v1, kling-v1-5, etc.

https://docs.newapi.pro

POST

`/kling/v1/videos/text2video`

Send

Authorization

Body

{% hint style="info" %}
使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`\
In: `header`
{% endhint %}

### Authorization

BearerAuth

AuthorizationBearer

### Request Body

Content type: application/json

Fields:

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

Example:

```
{
  "task_id": "abcd1234efgh",
  "status": "queued"
}
```

#### 400 application/json

Example:

```
{
  "error": {
    "message": "string",
    "type": "string",
    "param": "string",
    "code": "string"
  }
}
```

### Examples

{% tabs %}
{% tab title="cURL" %}
```
curl -X POST "https://docs.newapi.pro/kling/v1/videos/text2video" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endtab %}

{% tab title="JavaScript" %}

{% endtab %}

{% tab title="Go" %}

{% endtab %}

{% tab title="Python" %}

{% endtab %}

{% tab title="Java" %}

{% endtab %}

{% tab title="C#" %}

{% endtab %}
{% endtabs %}

Last updated on 3/1/2026

For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

Related links:

* [User Guide](https://docs.newapi.pro/en/docs)
* [Installation](https://docs.newapi.pro/en/docs/installation)
* [API Reference](https://docs.newapi.pro/en/docs/api)
* [AI Applications](https://docs.newapi.pro/en/docs/apps)
* [Skills](https://docs.newapi.pro/en/docs/skills)
* [Help & Support](https://docs.newapi.pro/en/docs/support)
* [Business Cooperation](https://docs.newapi.pro/en/docs/business)
