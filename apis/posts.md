---
layout: apis
title: Posts API
permalink: /api/posts/
api: true
posts: true
---

#### Create new post

    POST /posts

**Parameters**

* `title` (*Required* | **string**) - The title of the new post
* `body_html` (*Required* | **string**) - The html body of the new post
* `organization_ids` (*Required* | **array**) - The ids of organizations which the new post will be posted to
* `attachment_ids` (*Optional* | **array**) - The ids of attachments which will be attached to the new post
* `delayed_sms_at` (*Optional* | **integer**) - The value of time as an integer number of seconds since the Epoch


#### Get a single post

    GET /posts/:id


#### Get the forms

Get the forms of a single post.

    GET /posts/:id/forms


#### Get the receipts

Get the receipts of a single post.

    GET /posts/:id/receipts


#### Get unread receipts

Get unread receipts of a single post.

    GET /posts/:id/unread_receipts


#### Get read receipts

Get read receipts of a single post.

    GET /posts/:id/read_receipts


#### Get comments

Get comments of a single post.

    GET /posts/:id/comments


#### Post a new comments

Post a new comment to a single post.

    POST /posts/:id/comments

**Parameters**

* `body` (*Required* | **string**) - The body of the new comment


#### Get a sms notification scheduler

Get a sms notification scheduler of a single post, return the lasted ran scheduler if there arent schedulers which didnt run.

    GET /posts/:id/sms_scheduler


#### Run a sms notification

Run a sms notification of a single post.

    POST /posts/:id/sms_notifications


#### Get a call notification scheduler

Get a call notification scheduler of a single post, return the lasted ran scheduler if there arent schedulers which didnt run.

    GET /posts/:id/call_scheduler


#### Run a call notification

Run a call notification of a single post.

    POST /posts/:id/call_notifications


