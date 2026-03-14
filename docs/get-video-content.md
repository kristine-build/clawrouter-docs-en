# Get Video Content

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

AI Model APIVideosSora

## Get Video Content

Retrieves the video file content for a completed video task.

This interface proxies and returns the video file stream.

https://docs.newapi.pro

Endpoint GET `/v1/videos/{task_id}/content`

Authorization BearerAuth

Authorization Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

Path Parameters

* task\_id\* string\
  视频任务 ID

Response Body

* 200 — video/mp4
* 404 — application/json

Examples

cURL

```
curl -X GET "https://loading/v1/videos/string/content"
```

Responses

200 / 404

```
"string"
```

Error (application/json)

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

Related

* https://docs.newapi.pro/en/docs/api/ai-model/videos/sora/getvideocontent#authorization
* https://docs.newapi.pro/en/docs/api/ai-model/videos/sora/getvideocontent#path-parameters
* https://docs.newapi.pro/en/docs/api/ai-model/videos/sora/getvideocontent#response-body

Other docs

* [User Guide](https://docs.newapi.pro/en/docs)
* [Installation](https://docs.newapi.pro/en/docs/installation)
* [API Reference](https://docs.newapi.pro/en/docs/api)
* [AI Applications](https://docs.newapi.pro/en/docs/apps)
* [Skills](https://docs.newapi.pro/en/docs/skills)
* [Help & Support](https://docs.newapi.pro/en/docs/support)
* [Business Cooperation](https://docs.newapi.pro/en/docs/business)
