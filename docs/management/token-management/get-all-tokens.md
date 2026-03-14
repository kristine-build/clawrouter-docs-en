# Get All Tokens

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

## Management API — Token management

### Get All Tokens

{% hint style="info" %}
🔐 Login Required (User Permission)
{% endhint %}

GET https://docs.newapi.pro/api/token/

Path

```
/api/token/
```

Query

* [Query Parameters](get-all-tokens.md#query-parameters)
  * p?integer
  * page\_size?integer

Response

* [Response Body](get-all-tokens.md#response-body)

#### 200

cURL

{% code title="curl" %}
```bash
curl -X GET "https://docs.newapi.pro/api/token/"
```
{% endcode %}

200

Empty
