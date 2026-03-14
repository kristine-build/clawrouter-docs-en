# Get Kling Image-to-Video Task Status

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model APIVideosKling

## Get Kling Image-to-Video Task Status

Query the status and results of a Kling image-to-video task.

Base URL https://docs.newapi.pro

Method GET

Endpoint `/kling/v1/videos/image2video/{task_id}`

Authorization BearerAuth

Authorization header format: `Authorization: Bearer sk-xxxxxx`

Use Bearer Token authentication. In: header

Path Parameters

* task\_id (string) — 任务 ID

Response Body

* 200 application/json
* 404 application/json

Example request

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X GET "https://docs.newapi.pro/kling/v1/videos/image2video/string" \
  -H "Authorization: Bearer "
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

Example successful response (200)

```json
{
  "task_id": "abcd1234efgh",
  "status": "completed",
  "url": "https://example.com/video.mp4",
  "format": "mp4",
  "metadata": {
    "duration": 5,
    "fps": 30,
    "width": 1280,
    "height": 720,
    "seed": 20231234
  },
  "error": {
    "code": 0,
    "message": "string"
  }
}
```

Example error response (404 / other errors)

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

Last updated on 3/1/2026

Related

* Kling Text-to-Video (create): https://docs.newapi.pro/en/docs/api/ai-model/videos/kling/createklingtext2video
* Get Kling Text-to-Video Task Status: https://docs.newapi.pro/en/docs/api/ai-model/videos/kling/getklingtext2video
