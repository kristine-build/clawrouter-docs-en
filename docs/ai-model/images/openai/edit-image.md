# Edit Image

Documentation renewed! For old docs, visit https://doc.newapi.pro/

AI Model API — Images — Openai

## Edit Image

Creates an edited or extended image given an original image and a prompt.

Endpoint POST https://docs.newapi.pro/v1/images/edits/

Authorization Bearer token in request header

Header Authorization: Bearer

Request body (multipart/form-data)

* image\* (file)\
  要编辑的图像。必须是有效的 PNG 文件，小于 4MB，并且是方形的。如果未提供遮罩，图像必须具有透明度，将用作遮罩.\
  Format: binary
* mask (file, optional)\
  附加图像，其完全透明区域（例如，alpha 为零的区域）指示 image 应编辑的位置。必须是有效的 PNG 文件，小于 4MB，并且尺寸与原始 image 相同。\
  Format: binary
* prompt\* (string)\
  所需图像的文本描述。最大长度为 1000 个字符。
* n (string, optional)\
  要生成的图像数。必须介于 1 和 10 之间。
* size (string, optional)\
  生成图像的大小。必须是 `256x256`、`512x512` 或 `1024x1024` 之一。
* response\_format (string, optional)\
  生成的图像返回的格式。必须是 `url` 或 `b64_json`。
* user (string, optional)\
  代表您的最终用户的唯一标识符，可以帮助 OpenAI 监控和检测滥用行为。了解更多: https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids
* model (string, optional)

Response

* 200 application/json

Examples

cURL

{% code title="curl" %}
```bash
curl -X POST "https://docs.newapi.pro/v1/images/edits/" \
  -H "Authorization: Bearer " \
  -F image="cmMtdXBsb2FkLTE2ODc4MzMzNDc3NTEtMjA=/31225951_59371037e9_small.png" \
  -F prompt="A cute baby sea otter wearing a beret."
```
{% endcode %}

Response example (200)

```json
{}
```

Related

* https://docs.newapi.pro
* API Reference pages:
  * User Guide: https://docs.newapi.pro/en/docs
  * Installation: https://docs.newapi.pro/en/docs/installation
  * API Reference: https://docs.newapi.pro/en/docs/api
  * AI Applications: https://docs.newapi.pro/en/docs/apps
  * Skills: https://docs.newapi.pro/en/docs/skills
  * Help & Support: https://docs.newapi.pro/en/docs/support
  * Business Cooperation: https://docs.newapi.pro/en/docs/business

Last updated on 3/1/2026
