# Get Model List

Documentation renewed! For old docs, visit https://doc.newapi.pro/

## Management API — Channel management

### Get Model List

{% hint style="info" %}
👨‍💼 Requires Admin Permissions (Admin)
{% endhint %}

Endpoint

* Method: POST
* URL: https://docs.newapi.pro
* Path: /api/channel/fetch\_models

Request

* Content-Type: application/json

Request Body schema (application/json)

* base\_url? string
* type? integer
* key? string

Reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-fetch\_models-post#request-body

Response

* 200 — Empty

Reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-fetch\_models-post#response-body

Example — cURL

{% code title="curl" %}
```bash
curl -X POST "https://docs.newapi.pro/api/channel/fetch_models" \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endcode %}

How is this guide?

* Good
* Bad

Last updated on 3/1/2026
