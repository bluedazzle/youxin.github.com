---
layout: apis
title: Password API
permalink: /api/password/
api: true
password: true
---

#### Request the reset\_password email or sms\_token

Request the email or sms\_token, and parameters can one of email and phone.

    POST /password

**Parameters**

* `email` (*Alternative* | **string**) - The email address
* `phone` (*Alternative* | **string**) - The phone number


#### Verify the sms_token

    GET /password/valid_token

**Parameters**

* `reset_sms_token` (*Required* | **string**) - The sms_token
* `phone` (*Required* | **string**) - The phone number


#### Update the password

    PUT /password

**Parameters**

* `reset_sms_token` (*Required* | **string**) - The sms_token
* `phone` (*Required* | **string**) - The phone number
* `password` (*Required* | **string**) - The new password
* `password_confirmation` (*Required* | **string**) - The confirmation of new password


