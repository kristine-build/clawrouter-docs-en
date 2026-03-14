# Create Token

For old docs, visit https://doc.newapi.pro/

Management API — Token management

## Create Token

{% hint style="info" %}
🔐 Login Required (User Permission)
{% endhint %}

Endpoint

* POST https://docs.newapi.pro/api/token/

Request body

* Content-Type: application/json
* Schema / details: https://docs.newapi.pro/en/docs/api/management/token-management/token-post#request-body

Response

* 200 — details: https://docs.newapi.pro/en/docs/api/management/token-management/token-post#response-body

Example (cURL)

```bash
curl -X POST "https://docs.newapi.pro/api/token/" \
  -H "Content-Type: application/json" \
  -d '{}'
```

200

* Empty

Last updated on 3/1/2026
