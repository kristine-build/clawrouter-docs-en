# Update User Settings

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

## Management API — User management

## Update User Settings

{% hint style="info" %}
🔐 Login Required (User Permission)
{% endhint %}

PUT https://docs.newapi.pro/api/user/setting

Request Body (application/json)

* notify\_type? string
* quota\_warning\_threshold? number
* webhook\_url? string
* notification\_email? string

Response Body

#### 200

cURL example:

{% code title="cURL" %}
```bash
curl -X PUT "https://docs.newapi.pro/api/user/setting" \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endcode %}

Last updated on 3/1/2026
