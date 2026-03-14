# User Registration

Documentation renewed! For old docs, visit https://doc.newapi.pro/

## User Registration

{% hint style="info" %}
🔓 No Authentication Required
{% endhint %}

Base URL: https://docs.newapi.pro

Method: POST

Endpoint:

```
/api/user/register
```

### Request Body

Content type: application/json

Fields:

* username? string
* password? string
* email? string
* verification\_code? string
* aff\_code? string

(See full request schema: https://docs.newapi.pro/en/docs/api/management/user-auth/user-register-post#request-body)

### Response Body

200

Example (cURL):

{% code title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/api/user/register" \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endcode %}

Response: Empty

(See full response details: https://docs.newapi.pro/en/docs/api/management/user-auth/user-register-post#response-body)

Last updated on 3/1/2026
