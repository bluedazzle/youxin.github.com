---
layout: apis
title: Conversations API
permalink: /api/conversations/
api: true
conversations: true
---

#### Create a new conversation

    POST /conversations

Parameters

* `participant_ids` (*required* | **array**) - The ids of the participants


#### Get a conversation

Get a conversation which the authenticated user participate in.

    GET /conversations/:id


#### Delete a single conversation

Delete a single conversation which created by the authenticated user.

    DELETE /conversations/:id


#### Get messages of a single conversation

Get messages of a single conversation which the authenticated user participate in.

    GET /conversations/:id/messages


#### Create a new message

Post a new message to a single conversation which the authenticated user participate in.

    POST /conversations/:id/messages

Parameters

* `body` (*required* | **string**) - The body of the message


#### Add new participants

Add new participants to conversation which created by the authenticated user.

    POST /conversations/:id/participants

Parameters

* `participant_ids` (*required* | **string**) - The ids of the new participants


#### Delete participants

Delete participants from conversation which created by the authenticated user.

    DELETE /conversations/:id/participants

Parameters

* `participant_ids` (*required* | **string**) - The ids of the participants which will be deleted form the conversation


