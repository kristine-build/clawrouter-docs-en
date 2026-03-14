# Generate Images

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API · Images · Openai

## Generate Images

Creates an image given a prompt. [Learn more](https://platform.openai.com/docs/guides/images).

POST `/`v1`/`images`/`generations`/`

Send

Authorization

Body

### Authorization

Bearer

AuthorizationBearer

In: `header`

### Request Body

application/json

* model? string\
  用于图像生成的模型。`dall-e-2`、`dall-e-3` 或 `gpt-image-1` 之一。默认为 `dall-e-2`，除非使用特定于 `gpt-image-1` 的参数。
* prompt\* string\
  所需图像的文本描述。`gpt-image-1` 的最大长度为 32000 个字符，`dall-e-2` 的最大长度为 1000 个字符，`dall-e-3` 的最大长度为 4000 个字符。
* n? integer\
  要生成的图像数量。必须介于 1 到 10 之间。对于 `dall-e-3`，仅支持 `n=1`。
* size? string\
  生成的图像的大小。对于 `gpt-image-1`，必须是 `1024x1024`、`1536x1024`（横向）、`1024x1536`（纵向）或 `自动`（默认值）之一，\
  对于 `dall-e-2`，必须是 `256x256`、`512x512` 或 `1024x1024` 之一，\
  对于 `dall-e-3`，必须是 `1024x1024`、`1792x1024` 或 `1024x1792` 之一。
* background? string\
  允许为生成的图像的背景设置透明度。此参数仅支持 `gpt-image-1`。必须是以下之一 `透明`、`不透明`或`自动`（默认值）。使用`自动`时，模型将自动确定图像的最佳背景。\
  如果`是透明`的，则输出格式需要支持透明度，因此应将其设置为 `png`（默认值）或 `webp`。
* moderation? string\
  控制 `gpt-image-1` 生成的图像的内容审核级别。必须为 `低` 以进行限制较少的筛选或 `自动`（默认值）。
* quality? string
* stream? string
* style? string
* user? string

### Response Body

#### 200 application/json

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X POST "https://docs.newapi.pro/v1/images/generations/" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "prompt": "string"
  }'
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

Example 200 response:

```json
{
  "created": 0,
  "data": [
    {
      "b64_json": "string",
      "url": "string"
    }
  ],
  "usage": {
    "total_tokens": 0,
    "input_tokens": 0,
    "output_tokens": 0,
    "input_tokens_details": {
      "text_tokens": 0,
      "image_tokens": 0
    }
  }
}
```

Last updated on 3/1/2026

Related pages:

* https://docs.newapi.pro/en/docs/api/ai-model/images/openai/post-v1-images-edits
* https://docs.newapi.pro/en/docs/api/ai-model/images/qwen/createimage
