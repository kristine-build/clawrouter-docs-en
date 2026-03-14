# Delete Token

Documentation renewed! For old docs, visit https://doc.newapi.pro/

Management API — Token management

## Delete Token

{% hint style="warning" %}
🔐 Login Required (User Permission)
{% endhint %}

DELETE

```
/api/token/{id}
```

Path

* For details: https://docs.newapi.pro/en/docs/api/management/token-management/token-id-delete#path-parameters

Path Parameters

* id\* integer

Response Body

* For details: https://docs.newapi.pro/en/docs/api/management/token-management/token-id-delete#response-body

#### 200

Empty

Example

{% code title="cURL" %}
```bash
curl -X DELETE "https://docs.newapi.pro/api/token/0"
```
{% endcode %}

Last updated on 3/1/2026

Related

* Get All Tokens: https://docs.newapi.pro/en/docs/api/management/token-management/token-get
* Get Specified Token: https://docs.newapi.pro/en/docs/api/management/token-management/token-id-get
