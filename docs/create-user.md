# Create User

{% hint style="warning" %}
👨‍💼 Requires Administrator Permissions (Admin)
{% endhint %}

POST https://docs.newapi.pro/api/user/

Body: application/json

Request schema: https://docs.newapi.pro/en/docs/api/management/user-management/user-post#request-body

Response schema: https://docs.newapi.pro/en/docs/api/management/user-management/user-post#response-body

### Responses

* 200 — Empty

### Example (cURL)

```
curl -X POST "https://docs.newapi.pro/api/user/" \
  -H "Content-Type: application/json" \
  -d '{}'
```

Last updated on 3/1/2026
