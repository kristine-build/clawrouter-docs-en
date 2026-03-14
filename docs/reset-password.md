# Reset Password

Documentation renewed! For old docs, visit https://doc.newapi.pro/

## Reset Password

{% hint style="info" %}
🔓 No Authentication Required
{% endhint %}

Base URL: https://docs.newapi.pro

Method: POST

Endpoint:

```
/`api`/`user`/`reset`
```

Send

Body

### Request Body

Content-Type: application/json

Fields:

* email? string
* token? string
* password? string

(See full request schema: https://docs.newapi.pro/en/docs/api/management/user-auth/user-reset-post#request-body)

### Response Body

Status: 200

(See full response details: https://docs.newapi.pro/en/docs/api/management/user-auth/user-reset-post#response-body)

Example — cURL

```
curl -X POST "https://docs.newapi.pro/api/user/reset" \
  -H "Content-Type: application/json" \
  -d '{}'
```

200 — Empty

How is this guide?

* Good
* Bad

Last updated on 3/1/2026

Related:

* User Registration: https://docs.newapi.pro/en/docs/api/management/user-auth/user-register-post
* Send Email Verification Code: https://docs.newapi.pro/en/docs/api/management/user-auth/verification-get
