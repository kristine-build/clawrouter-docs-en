# Enable 2FA

Documentation renewed! For old docs, visit https://doc.newapi.pro/

Management API — Two factor auth

## Enable 2FA

{% hint style="warning" %}
🔐 Login Required (User Permission)
{% endhint %}

Endpoint

* POST https://docs.newapi.pro/api/user/2fa/enable

Request

* Content-Type: application/json

Request Body schema

* code? string

Raw example

```bash
curl -X POST "https://docs.newapi.pro/api/user/2fa/enable" \
  -H "Content-Type: application/json" \
  -d '{}'
```

Response

#### 200

Empty

Last updated on 3/1/2026

Related

* https://docs.newapi.pro/en/docs/api/management/two-factor-auth/user-2fa-disable-post
* https://docs.newapi.pro/en/docs/api/management/two-factor-auth/user-2fa-setup-post
