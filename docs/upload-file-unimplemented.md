# Upload File (Unimplemented)

{% hint style="warning" %}
This interface has not been implemented.
{% endhint %}

Endpoint

* POST https://docs.newapi.pro/v1/files

Authorization

* BearerAuth
* Header: Authorization: Bearer
* 使用 Bearer Token 认证。格式: `Authorization: Bearer sk-xxxxxx`
* In: `header`

Request Body

* Content type: multipart/form-data
* Fields:
  * file?file — Format: `binary`
  * purpose?string

Response Body

* Status: 501 application/json

Example cURL

```
curl -X POST "https://docs.newapi.pro/v1/files" \
  -H "Authorization: Bearer "
```

Example error response (501)

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

Related links

* Documentation home (old docs): https://doc.newapi.pro/
* API docs: https://docs.newapi.pro/en/docs/api
* Request body reference: https://docs.newapi.pro/en/docs/api/ai-model/unimplemented/files/createfile#request-body
* Authorization reference: https://docs.newapi.pro/en/docs/api/ai-model/unimplemented/files/createfile#authorization

Last updated on 3/1/2026
