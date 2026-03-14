# Admin Disable User 2FA

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

Management API — User management

## Admin Disable User 2FA

{% hint style="warning" %}
👨‍💼 Admin Permissions Required (Admin)
{% endhint %}

Endpoint

* Base URL: https://docs.newapi.pro
* Method: DELETE
* Path: `/api/user/{id}/2fa`

Request example

{% code title="cURL" %}
```bash
curl -X DELETE "https://docs.newapi.pro/api/user/0/2fa"
```
{% endcode %}

Path parameters

* id\* integer

Response body

* 200 — Empty

Last updated on 3/1/2026

Related

* https://docs.newapi.pro/en/docs/api/management/user-management/user-get
* https://docs.newapi.pro/en/docs/api/management/user-management/user-id-delete
