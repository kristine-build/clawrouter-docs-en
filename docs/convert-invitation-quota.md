# Convert Invitation Quota

{% hint style="warning" %}
🔐 Login Required (User Permission)
{% endhint %}

POST https://docs.newapi.pro/api/user/aff\_transfer

Request content type: application/json

## Request Body

See: https://docs.newapi.pro/en/docs/api/management/user-management/user-aff\_transfer-post#request-body

Schema (application/json)

quota?integer

## Response

See: https://docs.newapi.pro/en/docs/api/management/user-management/user-aff\_transfer-post#response-body

200 — Empty

## Example

curl

```
curl -X POST "https://docs.newapi.pro/api/user/aff_transfer" \
  -H "Content-Type: application/json" \
  -d '{}'
```

Last updated on 3/1/2026
