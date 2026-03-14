# Manage User Status

Documentation renewed! For old docs, visit https://doc.newapi.pro/

https://docs.newapi.pro

## Manage User Status

👨‍💼 Admin privileges required

POST https://docs.newapi.pro/api/user/manage

Send

Request body (application/json)

* id? integer
* action? string\
  Value in `"disable" | "enable" | "delete" | "promote" | "demote"`

More details: https://docs.newapi.pro/en/docs/api/management/user-management/user-manage-post#request-body

Response

* 200 — Empty

More details: https://docs.newapi.pro/en/docs/api/management/user-management/user-manage-post#response-body

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/api/user/manage" \
  -H "Content-Type: application/json" \
  -d '{}'
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
// JavaScript example
```
{% endtab %}

{% tab title="Go" %}
```go
// Go example
```
{% endtab %}

{% tab title="Python" %}
```python
# Python example
```
{% endtab %}

{% tab title="Java" %}
```java
// Java example
```
{% endtab %}

{% tab title="C#" %}
```csharp
// C# example
```
{% endtab %}
{% endtabs %}

How is this guide?

GoodBad

Last updated on 3/1/2026
