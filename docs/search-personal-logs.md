# Search Personal Logs

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

Management API — Logs

## Search Personal Logs

🔐 Login Required (User Permission)

Endpoint GET https://docs.newapi.pro/api/log/self/search

Request GET `/api/log/self/search`

Query

* keyword? string

Response

#### 200

cURL

{% code title="cURL" %}
```bash
curl -X GET "https://docs.newapi.pro/api/log/self/search"
```
{% endcode %}

Notes

{% hint style="info" %}
This endpoint requires the user to be logged in and have the appropriate permission.
{% endhint %}

Last updated on 3/1/2026

Links

* [Documentation home](https://docs.newapi.pro/)
* [Query Parameters reference](search-personal-logs.md#query-parameters)
* [Response Body reference](search-personal-logs.md#response-body)
