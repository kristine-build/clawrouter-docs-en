# Add Channel

Documentation renewed! For old docs, visit https://doc.newapi.pro/

## Management API — Channel management

### Add Channel

{% hint style="warning" %}
👨‍💼 Requires Admin Permissions
{% endhint %}

POST https://docs.newapi.pro/api/channel/

Request Content-Type: application/json

Body

* mode? string\
  Value in `"single" | "batch" | "multi_to_single"`
* channel? object\
  Unresolved $ref: #/definitions/224188811

Request Body reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-post#request-body

Response Body reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-post#response-body

#### Example

{% tabs %}
{% tab title="cURL" %}
```
curl -X POST "https://docs.newapi.pro/api/channel/" \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endtab %}

{% tab title="JavaScript" %}

{% endtab %}

{% tab title="Go" %}

{% endtab %}

{% tab title="Python" %}

{% endtab %}

{% tab title="Java" %}

{% endtab %}

{% tab title="C#" %}

{% endtab %}
{% endtabs %}

Response: 200

Body: Empty

Last updated on 3/1/2026
