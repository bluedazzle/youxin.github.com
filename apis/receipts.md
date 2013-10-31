---
layout: apis
title: Receipts API
permalink: /api/receipts/
api: true
receipts: true
---

#### Get receipts

Get receipts which the authenticated user received

    GET /receipts


#### Get a single receipt

    GET /receipts/:id


#### Favorite a single receipt

    POST /receipts/:id/favorite


#### Unfavorite a single receipt

    DELETE /receipts/:id/favorite


#### Read a single receipt

Mark a single receipt as read

    PUT /receipts/:id/read


