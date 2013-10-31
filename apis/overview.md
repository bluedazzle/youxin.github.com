---
layout: apis
title: Overview
permalink: /api/overview/
api: true
overview: true
---

### API version

**host**: `https://combee.co`

**api_version**: `v1`


### Authentication

All APIs implement base on token authentication, and follow REST architectural style.

Login to get `private_token`, and append `private_token=<private_token>` to url params to all URIs which request authentication, or add HTTP_PRIVATE_TOKEN header.

Eg:

```
GET /api/v1/user?prvate_token=<prvate_token> HTTP/1.1
Host: combee.co
Cache-Control: no-cache
```

*or*

```
GET /api/v1/user HTTP/1.1
Host: combee.co
HTTP_PRIVATE_TOKEN: <private_token>
Cache-Control: no-cache
```

### Common

#### paginate

Paginater can be use in the most array responses.

* `page` - The page number
* `per_page` - The number of records per page
* `since_id` - The id of records greater than `since_id`
* `max_id` - The id of records less than `max_id`


#### Errors

HTTP status code Definitions in APIs. [definitions](http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html)

* `400` - Bad request, there is some wrong with the parameters.
* `401` - Unauthorized, the resource needs authentication, and `private_token` isnt correct.
* `403` - Forbidden, the authorized user doesnt have the authorization.
* `404` - Not found, the resource not found.


