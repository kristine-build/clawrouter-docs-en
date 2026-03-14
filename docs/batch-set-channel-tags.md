# Batch Set Channel Tags

Management API — Channel management

## Batch Set Channel Tags

👨‍💼 Requires Administrator Permissions (Admin)

Endpoint POST `/`api`/`channel`/`batch`/`tag\`

Base URL: https://docs.newapi.pro

Request Body Content-Type: application/json

Fields

* ids? array
* tag? string

Response

* 200 — Empty

Example (cURL)

```bash
curl -X POST "https://docs.newapi.pro/api/channel/batch/tag" \
  -H "Content-Type: application/json" \
  -d '{}'
```

Related

* Old docs: https://doc.newapi.pro/
* Management — Batch Delete Channels: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-batch-post
* Management — Copy Channel: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-copy-id-post

Last updated on 3/1/2026
