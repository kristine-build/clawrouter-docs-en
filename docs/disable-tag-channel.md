# Disable Tag Channel

Documentation renewed! For old docs, visit https://doc.newapi.pro/

## Management API — Channel management

### Disable Tag Channel

{% hint style="warning" %}
👨‍💼 Admin privileges required
{% endhint %}

Endpoint

* Method: POST
* URL: https://docs.newapi.pro/api/channel/tag/disabled

Request body (application/json)

See detailed schema: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-tag-disabled-post#request-body

Body fields

* tag? string

Example cURL

```bash
curl -X POST "https://docs.newapi.pro/api/channel/tag/disabled" \
  -H "Content-Type: application/json" \
  -d '{}'
```

Response

See detailed response: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-tag-disabled-post#response-body

* 200 — Empty

Misc

* How is this guide? Good / Bad
* Last updated on 3/1/2026
