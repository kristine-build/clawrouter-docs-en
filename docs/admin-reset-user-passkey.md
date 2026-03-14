# Admin Reset User Passkey

Management API — User management

{% hint style="info" %}
👨‍💼 Requires Admin Permissions (Admin)
{% endhint %}

DELETE https://docs.newapi.pro

Endpoint

```
/api/user/{id}/reset_passkey
```

Path

Path Parameters

* id — integer (required)

More details:

* https://docs.newapi.pro/en/docs/api/management/user-management/user-id-reset\_passkey-delete#path-parameters

Response Body

### 200

Empty

Reference:

* https://docs.newapi.pro/en/docs/api/management/user-management/user-id-reset\_passkey-delete#response-body

Example

cURL

{% code title="curl" %}
```bash
curl -X DELETE "https://docs.newapi.pro/api/user/0/reset_passkey"
```
{% endcode %}

Last updated on 3/1/2026
