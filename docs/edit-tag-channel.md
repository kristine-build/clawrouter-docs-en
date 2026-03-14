# Edit Tag Channel

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

## Management API — Channel management

### Edit Tag Channel

{% hint style="info" %}
👨‍💼 Requires Administrator Permissions (Admin)
{% endhint %}

Method: PUT

Endpoint:

```
/`api`/`channel`/`tag`
```

Base URL:

```
https://docs.newapi.pro
```

Send Body: application/json

Request Body (fields)

* tag?string
* new\_tag?string
* priority?integer
* weight?integer

Reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-tag-put#request-body

Response Body

* 200 — Empty

Reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-tag-put#response-body

Example — cURL

{% code title="curl" %}
```bash
curl -X PUT "https://docs.newapi.pro/api/channel/tag" \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endcode %}

Last updated on 3/1/2026
