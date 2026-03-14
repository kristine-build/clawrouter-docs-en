# Start Passkey Login

Documentation renewed! For old docs, visit https://doc.newapi.pro/

## Start Passkey Login

{% hint style="info" %}
No Authentication Required
{% endhint %}

Endpoint POST https://docs.newapi.pro/api/user/passkey/login/begin

Request POST /`api`/`user`/`passkey`/`login`/`begin`

cURL example:

{% code title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/api/user/passkey/login/begin"
```
{% endcode %}

Response Body See: https://docs.newapi.pro/en/docs/api/management/user-auth/user-passkey-login-begin-post#response-body

* 200 — Empty

Last updated on 3/1/2026

Related

* Complete Passkey Login (POST): https://docs.newapi.pro/en/docs/api/management/user-auth/user-passkey-login-finish-post
* User Logout (GET): https://docs.newapi.pro/en/docs/api/management/user-auth/user-logout-get
