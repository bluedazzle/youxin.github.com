---
layout: apis
title: Notifications API
permalink: /api/notifications/
api: true
notifications: true
---

#### Read a single notification

Mark a single notification as read.

    PUT /notifications/:id/read


#### Read notifications

Mark some notifications as read.

    PUT /notifications/read

**Parameters**

* `notification_ids` (*Required* | **array**) - The ids of notifications


