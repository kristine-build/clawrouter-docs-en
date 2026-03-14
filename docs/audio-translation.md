# Audio Translation

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

AI Model APIAudioOpenai

## Audio Translation

Translates audio into English text

https://docs.newapi.pro

POST

`/v1/audio/translations`

Send

Authorization

Body

### Authorization

BearerAuth

AuthorizationBearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

### Request Body

Content type: multipart/form-data

* file\* — file\
  Format: `binary`
* model\* — string
* prompt? — string
* response\_format? — string
* temperature? — number

### Response Body

#### 200 application/json

Response example:

```
{
  "text": "string"
}
```

### Examples

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/v1/audio/translations" \
  -H "Authorization: Bearer " \
  -F file="string" \
  -F model="string"
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
// JavaScript example (from source)
```
{% endtab %}

{% tab title="Go" %}
```go
// Go example (from source)
```
{% endtab %}

{% tab title="Python" %}
```python
# Python example (from source)
```
{% endtab %}

{% tab title="Java" %}
```java
// Java example (from source)
```
{% endtab %}

{% tab title="C#" %}
```csharp
// C# example (from source)
```
{% endtab %}
{% endtabs %}

Last updated on 3/1/2026
