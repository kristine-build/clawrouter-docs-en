# Get Kling Text-to-Video Task Status

AI Model APIVideosKling

## Get Kling Text-to-Video Task Status

Query the status and results of a Kling text-to-video task.

https://docs.newapi.pro

GET

\`\`/`kling`/`v1`/`videos`/`text2video`/`{task_id}`

Send

Authorization

Path

### Authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### Path Parameters

task\_id _string_\
任务 ID

### Response Body

<details>

<summary>200 application/json</summary>

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

</details>

<details>

<summary>404 application/json</summary>

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

</details>

### Example (cURL)

```
curl -X GET "https://docs.newapi.pro/kling/v1/videos/text2video/string" \
  -H "Authorization: Bearer "
```

How is this guide?

GoodBad

Last updated on 3/1/2026

Related:

* https://docs.newapi.pro/en/docs
* https://docs.newapi.pro/en/docs/installation
* https://docs.newapi.pro/en/docs/api
* https://docs.newapi.pro/en/docs/apps
* https://docs.newapi.pro/en/docs/skills
* https://docs.newapi.pro/en/docs/support
* https://docs.newapi.pro/en/docs/business

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)
