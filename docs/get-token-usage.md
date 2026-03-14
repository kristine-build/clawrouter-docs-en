# Get Token Usage

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

Management API — Token management

## Get Token Usage

🔑 Token Authentication Required (TokenAuth)

Endpoint GET https://docs.newapi.pro/api/usage/token/

Description Returns usage information for the current bearer token.

Authorization

{% hint style="info" %}
Use Bearer Token authentication.

Format: Authorization: Bearer sk-xxxxxx

Header name: Authorization (in: header)
{% endhint %}

Header Parameters

* Authorization? string

Response Body

#### 200

Empty

Example request (cURL)

```bash
curl -X GET "https://docs.newapi.pro/api/usage/token/" \
  -H "Authorization: Bearer "
```

References

* [Authorization](get-token-usage.md#authorization)
* [Header Parameters](get-token-usage.md#header-parameters)
* [Response Body](get-token-usage.md#response-body)

Last updated on 3/1/2026
