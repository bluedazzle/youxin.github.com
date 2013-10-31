---
layout: apis
title: Users API
permalink: /api/users/
api: true
users: true
---

### User


#### Get the authenticated user

    GET /user

#### Update the authenticated user

    PUT /user

**Parameters**

* `phone` (*Required* | **string**) - Valid phone starting with 1 (regex `/\A1\d+\Z/`)
* `avatar` (*Optional* | **file**) - New avatar picture
* `header` (*Optional* | **file**) - New header picture
* `name` (*Optional* | **string**) - Valid name with length in 2..10
* `bio` (*Optional* | **string**) - Biography of user
* `gender` (*Optional* | **string**) - Valid gender (inclusion [男, 女])
* `qq` (*Optional* | **string**) - QQ number with length in 5..11 (regex `/\A\d{5,11}\Z/`)
* `blog` (*Optional* | **string**) - Blog address
* `uid` (*Optional* | **string**) - Valid user id (ie: student id)
* `email` (*Optional* | **string**) - Valid email address


#### Get authorized organizations

Get authorized organizations of the authenticated user.

    GET /user/authorized_organizations

**Parameters**

* `actions` (*Optional* | **array**) - Specify actions


#### Get recent organizations

Get recent organizations which have send at least a post to the authenticated user.

    GET /user/receipt_organizations


#### Get recent users

Get recent users which have send at least a post to the authenticated user.

    GET /user/receipt_users



#### Get receipts

Get all receipts of the authenticated user.

    GET /user/receipts



#### Get unread receipts

Get all unread receipts of the authenticated user.

    GET /user/unread_receipts



#### Get favorited receipts

Get all favorited receipts of the authenticated user.

    GET /user/favorited_receipts



#### Create an ios device token

Create an iOS device token of the authenticated user (*iOS only*).

    POST /user/ios_device_token

**Parameters**

* `device_token` (*Required* | **string**) - Valid ios_device_token (regex `\A[a-z0-9]{64}\z`)


#### Delete an ios device token

Delete an iOS device token of the authenticated user (*iOS only*).

    Delete /user/ios_device_token

**Parameters**

* `device_token` (*Required* | **string**) - Valid ios_device_token (regex `\A[a-z0-9]{64}\z`)


#### Get conversations

Get conversations of the authenticated user.

    GET /user/conversations


#### Get notifications

Get unread notifications count and notification_channel (*Android only*) of the authenticated user.

    GET /user/notifications


#### Get notifications timeline

Get notifications of the authenticated user.

    GET /user/notifications_timeline


#### Get unread notifications timeline

Get unread notifications of the authenticated user.

    GET /user/notifications_timeline/unread


#### Get comment notifications timeline

Get comment notifications of the authenticated user.

    GET /user/comment_notifications


#### Get unread comment notifications timeline

Get unread comment notifications of the authenticated user.

    GET /user/comment_notifications/unread


#### Get organization notificationstimeline

Get organization notifications of the authenticated user.

    GET /user/organization_notifications


#### Get unread organization notifications timeline

Get unread organization notifications of the authenticated user.

    GET /user/organization_notifications/unread


#### Get message notifications timeline

Get message notifications of the authenticated user.

    GET /user/message_notifications


#### Get unread message notifications timeline

Get unread message notifications of the authenticated user.

    GET /user/message_notifications/unread


### Users


#### Get a single user

    GET /users/:id


#### Get organizations

Get organizations of a single user

    GET /users/:id/organizations


#### Get receipts

Get receipts from a single user

    GET /users/:id/receipts


#### Get unread receipts

Get unread receipts from a single user

    GET /users/:id/unread_receipts


