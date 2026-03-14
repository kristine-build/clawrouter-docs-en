# Get All Channels

Management API — Channel management

## Get All Channels

{% hint style="info" %}
Requires Administrator Permissions (Admin)
{% endhint %}

GET

Endpoint:

```
/`api`/`channel`/
```

Base URL: https://docs.newapi.pro

Send

Query

Query parameters

* p?integer
* page\_size?integer
* id\_sort?boolean
* tag\_mode?boolean
* status?string
* type?integer

Reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-get#query-parameters

Response Body

Reference: https://docs.newapi.pro/en/docs/api/management/channel-management/channel-get#response-body

#### 200

Example cURL

{% code title="cURL" %}
```bash
curl -X GET "https://docs.newapi.pro/api/channel/"
```
{% endcode %}

200

Empty

How is this guide?

* Good
* Bad

Last updated on 3/1/2026

Related

* Fix Channel Capability (POST): https://docs.newapi.pro/en/docs/api/management/channel-management/channel-fix-post
* Delete Channel (DELETE): https://docs.newapi.pro/en/docs/api/management/channel-management/channel-id-delete

Documentation renewed! For old docs, visit: https://doc.newapi.pro

Other docs

* User Guide: https://docs.newapi.pro/en/docs
* Installation: https://docs.newapi.pro/en/docs/installation
* API Reference: https://docs.newapi.pro/en/docs/api
* AI Applications: https://docs.newapi.pro/en/docs/apps
* Skills: https://docs.newapi.pro/en/docs/skills
* Help & Support: https://docs.newapi.pro/en/docs/support
* Business Cooperation: https://docs.newapi.pro/en/docs/business
