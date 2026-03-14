# Copy Channel

Management API — Channel management

## Copy Channel

👨‍💼 Requires Administrator Privileges (Admin)

POST /api/channel/copy/{id}

Endpoint

```
POST `/api/channel/copy/{id}`
```

Path parameters

* id — integer (required)

Query parameters

* suffix — string (optional)
* reset\_balance — boolean (optional)

Response Body

#### 200

Empty

Code samples

{% tabs %}
{% tab title="cURL" %}
```
curl -X POST "https://docs.newapi.pro/api/channel/copy/0"
```
{% endtab %}
{% endtabs %}

Last updated on 3/1/2026

Related

* Batch Set Channel Tags: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-batch-tag-post
* Delete Disabled Channels: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-disabled-delete
