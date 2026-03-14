# Kling Image to Video

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model APIVideosKling

## Kling — Image to Video

Generate video from images using the Kling model.

Supports passing image URLs or Base64 encoded image data via the `image` parameter.

Endpoint

* POST https://docs.newapi.pro/kling/v1/videos/image2video
* Path: `/kling/v1/videos/image2video`

Authorization

* BearerAuth
* Header: Authorization: Bearer
* 使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`
* In: header

Request Body (application/json)

* model? string — 模型/风格 ID
* prompt? string — 文本描述提示词
* image? string — 图片输入 (URL 或 Base64)
* duration? number — 视频时长（秒）
* width? integer — 视频宽度
* height? integer — 视频高度
* fps? integer — 视频帧率
* seed? integer — 随机种子
* n? integer — 生成视频数量
* response\_format? string — 响应格式
* user? string — 用户标识
* metadata? object — 扩展参数 (如 negative\_prompt, style, quality\_level 等)

Response Body

200 application/json

* Example:

```
{
  "task_id": "abcd1234efgh",
  "status": "queued"
}
```

400 application/json

* Example:

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

Code samples

{% tabs %}
{% tab title="cURL" %}
```
curl -X POST "https://docs.newapi.pro/kling/v1/videos/image2video" \
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

Notes

* Supports image input as URL or Base64.
* 用法与参数详见 Request Body 字段说明。

Last updated on 3/1/2026

Original docs: https://docs.newapi.pro/en/docs/api/ai-model/videos/kling/createklingimage2video
