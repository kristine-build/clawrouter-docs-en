# Get Video Generation Task Status

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

AI Model APIVideos

## Get Video Generation Task Status

Query the status and results of a video generation task.

Task Status:

* `queued`: Queued
* `in_progress`: In progress
* `completed`: Completed
* `failed`: Failed

https://docs.newapi.pro

GET

\`\`/`v1`/`video`/`generations`/`{task_id}`

Send

Authorization

Path

### [Authorization](get-video-generation-task-status.md#authorization)

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### [Path Parameters](get-video-generation-task-status.md#path-parameters)

task\_id \* string

任务 ID

### [Response Body](get-video-generation-task-status.md#response-body)

#### 200 application/json

Example successful response:

```
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

#### 404 application/json

Example error response:

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
```bash
curl -X GET "https://docs.newapi.pro/v1/video/generations/string" \
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

Last updated on 3/1/2026

Related:

* [Create Video Generation TaskPOST\ \ Previous Page](create-video-generation-task.md)
* [Jimeng Video GenerationPOST\ \ Next Page](/broken/pages/1995a265f86a17934e5711bda6f0180be1a2b920)
