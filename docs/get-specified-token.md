# Get Specified Token

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

## Management API — Token management

### Get Specified Token

{% hint style="info" %}
🔐 Login Required (User Permission)
{% endhint %}

Endpoint GET https://docs.newapi.pro

Path \`\`/`api`/`token`/`{id}`

Send

Path parameters For details see: https://docs.newapi.pro/en/docs/api/management/token-management/token-id-get#path-parameters

* id \*integer

Response body For details see: https://docs.newapi.pro/en/docs/api/management/token-management/token-id-get#response-body

#### 200

cURL example \{% code title="curl" %\}

```bash
curl -X GET "https://docs.newapi.pro/api/token/0"
```

Response: 200 Empty

Last updated on 3/1/2026
