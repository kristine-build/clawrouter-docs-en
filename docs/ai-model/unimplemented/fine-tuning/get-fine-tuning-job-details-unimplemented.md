# Get Fine-tuning Job Details (Unimplemented)

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

AI Model API — Unimplemented — Fine tuning

Get Fine-tuning Job Details (Unimplemented) This interface is not yet implemented

Endpoint GET `/v1/fine-tunes/{fine_tune_id}`

Base URL https://docs.newapi.pro

Authorization BearerAuth

Use Bearer Token authentication. Format: Authorization: Bearer sk-xxxxxx

In: header

Example header:

```
Authorization: Bearer <token>
```

Path Parameters

* fine\_tune\_id\* (string)

Response Body

501 — application/json

Example cURL request:

```
curl -X GET "https://docs.newapi.pro/v1/fine-tunes/string" \
  -H "Authorization: Bearer "
```

501 Example response:

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

Last updated on 3/1/2026

Related

* Create Video Generation Task (unrelated page link removed)
* List Fine-tuning Jobs (unimplemented) — source: https://docs.newapi.pro/en/docs/api/ai-model/unimplemented/fine-tuning/listfinetunes

(Original documentation links)

* User Guide: https://docs.newapi.pro/en/docs
* Installation: https://docs.newapi.pro/en/docs/installation
* API Reference: https://docs.newapi.pro/en/docs/api
* AI Applications: https://docs.newapi.pro/en/docs/apps
* Skills: https://docs.newapi.pro/en/docs/skills
* Help & Support: https://docs.newapi.pro/en/docs/support
* Business Cooperation: https://docs.newapi.pro/en/docs/business
