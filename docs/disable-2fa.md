# Disable 2FA

Management API — Two factor auth

## Disable 2FA

{% hint style="info" %}
🔐 Login required (User permission)
{% endhint %}

Endpoint

POST https://docs.newapi.pro/api/user/2fa/disable

Request

Content-Type: application/json

Request body schema

application/json

* code? string

Response

200

Empty

Example

```bash
curl -X POST "https://docs.newapi.pro/api/user/2fa/disable" \
  -H "Content-Type: application/json" \
  -d '{}'
```

References

* Request Body: https://docs.newapi.pro/en/docs/api/management/two-factor-auth/user-2fa-disable-post#request-body
* Response Body: https://docs.newapi.pro/en/docs/api/management/two-factor-auth/user-2fa-disable-post#response-body

Documentation renewed! For old docs, visit https://doc.newapi.pro/

Related pages

* User Guide: https://docs.newapi.pro/en/docs
* Installation: https://docs.newapi.pro/en/docs/installation
* API Reference: https://docs.newapi.pro/en/docs/api
* AI Applications: https://docs.newapi.pro/en/docs/apps
* Skills: https://docs.newapi.pro/en/docs/skills
* Help & Support: https://docs.newapi.pro/en/docs/support
* Business Cooperation: https://docs.newapi.pro/en/docs/business

Last updated on 3/1/2026
