# Initialize System

## Initialize System

🔓 No Authentication Required

Endpoint

* POST https://docs.newapi.pro/api/setup

Request body

* Content type: application/json
* Fields:
  * username? string
  * password? string

Request body details: https://docs.newapi.pro/en/docs/api/management/system/setup-post#request-body

Response body details: https://docs.newapi.pro/en/docs/api/management/system/setup-post#response-body

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/api/setup" \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endtab %}
{% endtabs %}

Response

* 200 — Empty

Last updated on 3/1/2026
