# Create Video Generation Task

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

AI Model APIVideos

## Create Video Generation Task

Submit a video generation task, supporting text-to-video and image-to-video.

Returns the task ID. The task status can be queried via the GET API.

https://docs.newapi.pro

POST

`/`v1`/`video`/`generations\`

Send

Authorization

Body

<details>

<summary>Authorization</summary>

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

</details>

<details>

<summary>Request Body</summary>

application/json

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

</details>

<details>

<summary>Response Body</summary>

#### 200 application/json

Example success response:

```
{
  "task_id": "abcd1234efgh",
  "status": "queued"
}
```

#### 400 application/json

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

</details>

cURL

```
curl -X POST "https://docs.newapi.pro/v1/video/generations" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{}'
```

JavaScript

Go

Python

Java

C#

Last updated on 3/1/2026
