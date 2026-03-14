# Authentication System Description (Auth)

Documentation renewed! For old docs, visit [doc.newapi.pro](https://doc.newapi.pro/)

[User Guide](https://docs.newapi.pro/en/docs) [Installation](https://docs.newapi.pro/en/docs/installation) [API Reference](https://docs.newapi.pro/en/docs/api) [AI Applications](https://docs.newapi.pro/en/docs/apps) [Skills](https://docs.newapi.pro/en/docs/skills) [Help & Support](https://docs.newapi.pro/en/docs/support) [Business Cooperation](https://docs.newapi.pro/en/docs/business)

## Management API

## Authentication System Description (Auth)

Description of backend management interface authentication methods and permission levels

### Description

Backend management interfaces adopt a multi-level authentication mechanism, commonly: **Public**, **User**, **Admin**, **Root**.

### Authentication Methods (Choose One)

#### Session

Obtain Session via the login interface:

* `POST /api/user/login`

#### Access Token (Recommended)

Carry in the request header:

```
Authorization: Bearer {token}
```

Tokens can be generated in "Personal Settings - Security Settings - System Access Tokens".

### Required Request Headers

Some interfaces require carrying a user identification request header:

```
New-Api-User: {user_id}
```

Where `{user_id}` must match the currently logged-in user.

### Permission Levels

* **Public**: No authentication required
* **User**: Requires login or Access Token
* **Admin**: Requires administrator privileges
* **Root**: Highest privilege
