# Enable Tag Channel

Documentation renewed! For old docs, visit https://doc.newapi.pro/

## Enable Tag Channel

{% hint style="warning" %}
👨‍💼 Requires Admin Permissions
{% endhint %}

POST

Endpoint

```
/`api`/`channel`/`tag`/`enabled`
```

Request

* Content-Type: application/json

Request body schema

```
tag? string
```

Example — cURL

```bash
curl -X POST "https://docs.newapi.pro/api/channel/tag/enabled" \
  -H "Content-Type: application/json" \
  -d '{}'
```

Response

* 200 — Empty body

Last updated on 3/1/2026

Related

* https://docs.newapi.pro/en/docs/api/management/channel-management/channel-tag-enabled-post#request-body
* https://docs.newapi.pro/en/docs/api/management/channel-management/channel-tag-enabled-post#response-body
