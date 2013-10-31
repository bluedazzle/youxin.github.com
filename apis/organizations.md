---
layout: apis
title: Organizations API
permalink: /api/organizations/
api: true
organizations: true
---

#### Get organizations

Get all organizations of the current namespace.

    GET /organizations


#### Get a single organization

    GET /organizations/:id


#### Update a single organization

    PUT /organizations/:id

**Parameters**

* `avatar` (*Optional* | **file**) - New avatar picture
* `header` (*Optional* | **file**) - New header picture
* `name` (*Required* | **string**) - Valid name
* `bio` (*Optional* | **string**) - Biography of organization


#### Get members

Get members of a single organization.

    GET /organizations/:id/members


#### Get receipts

Get receipts which from a single organization.

    GET /organizations/:id/receipts


#### Get unread receipts

Get unread receipts which from a single organization.

    GET /organizations/:id/unread_receipts


#### Get children

Get children of a single organization.

    GET /organizations/:id/children


#### Get authorized users

Get users who has authorizations in a single organization.

    GET /organizations/:id/authorized_users


