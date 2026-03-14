# Delete File (Unimplemented)

This interface is not yet implemented.

Endpoint:\
DELETE https://docs.newapi.pro/`/v1`/`files`/`{file_id}`

## Authorization

BearerAuth

Format: `Authorization: Bearer sk-xxxxxx`\
使用 Bearer Token 认证。\
In: header

## Path Parameters

* file\_id (string) — required

## Response Body

### 501 application/json

```json
{
  "error": {
    "message": "string",
    "type": "string",
    "param": "string",
    "code": "string"
  }
}
```

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X DELETE "https://docs.newapi.pro/v1/files/string" \
  -H "Authorization: Bearer "
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
// JavaScript sample placeholder (unimplemented)
```
{% endtab %}

{% tab title="Go" %}
```go
// Go sample placeholder (unimplemented)
```
{% endtab %}

{% tab title="Python" %}
```python
# Python sample placeholder (unimplemented)
```
{% endtab %}

{% tab title="Java" %}
```java
// Java sample placeholder (unimplemented)
```
{% endtab %}

{% tab title="C#" %}
```csharp
// C# sample placeholder (unimplemented)
```
{% endtab %}
{% endtabs %}

Last updated on 3/1/2026

For related endpoints:

* Upload File (Unimplemented): https://docs.newapi.pro/en/docs/api/ai-model/unimplemented/files/createfile
* Get File Content (Unimplemented): https://docs.newapi.pro/en/docs/api/ai-model/unimplemented/files/downloadfile

External docs (old): https://doc.newapi.pro/
