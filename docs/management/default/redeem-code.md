# Redeem Code

🔐 Login Required (User Permission)

Endpoint POST https://docs.newapi.pro/api/user/topup

Path `/`api`/`user`/`topup\`

Authorization BearerAuth

Authorization: Bearer

使用 Bearer Token 认证。\
格式: `Authorization: Bearer sk-xxxxxx`

In: `header`

Request Body Content-Type: application/json

* key\* string

Example request (cURL)

```
curl -X POST "https://docs.newapi.pro/api/user/topup" \
  -H "Authorization: Bearer " \
  -H "Content-Type: application/json" \
  -d '{
    "key": "string"
  }'
```

Note: The original page lists the following languages/formats for examples: cURL JavaScript Go Python Java C#

Response Body

### 200 application/json

Example response:

```
{}
```

Last updated on 3/1/2026

Related links

* https://docs.newapi.pro
* https://docs.newapi.pro/en/docs/api/management/channel-management/channel-update\_balance-id-get
* https://docs.newapi.pro/en/docs/api/management/groups/group-get
* https://docs.newapi.pro/en/docs
* https://docs.newapi.pro/en/docs/installation
* https://docs.newapi.pro/en/docs/api
* https://docs.newapi.pro/en/docs/apps
* https://docs.newapi.pro/en/docs/skills
* https://docs.newapi.pro/en/docs/support
* https://docs.newapi.pro/en/docs/business

Documentation renewed! For old docs, visit https://doc.newapi.pro/
