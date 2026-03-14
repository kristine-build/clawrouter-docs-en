# Manage Multiple Keys

> POST https://docs.newapi.pro/api/channel/multi\_key/manage

{% hint style="info" %}
👨‍💼 Admin privileges required
{% endhint %}

Request Content-Type: application/json

## Request Body

Fields:

* channel\_id? integer
* action? string\
  Value in `"get_key_status" | "disable_key" | "enable_key" | "delete_key" | "delete_disabled_keys" | "enable_all_keys" | "disable_all_keys"`
* key\_index? integer

(See original request spec: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-multi\_key-manage-post#request-body)

## Example cURL

```bash
curl -X POST "https://docs.newapi.pro/api/channel/multi_key/manage" \
  -H "Content-Type: application/json" \
  -d '{}'
```

## Response

200 — Empty

(See original response spec: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-multi\_key-manage-post#response-body)

## Related links

* Documentation renewed homepage: https://doc.newapi.pro/
* User Guide: https://docs.newapi.pro/en/docs
* Installation: https://docs.newapi.pro/en/docs/installation
* API Reference: https://docs.newapi.pro/en/docs/api
* AI Applications: https://docs.newapi.pro/en/docs/apps
* Skills: https://docs.newapi.pro/en/docs/skills
* Help & Support: https://docs.newapi.pro/en/docs/support
* Business Cooperation: https://docs.newapi.pro/en/docs/business

Last updated on 3/1/2026
