---
layout: apis
title: Forms API
permalink: /api/forms/
api: true
forms: true
---

#### Get a single form

    GET /forms/:id


#### Post a new collection

Create a collection to a single form.
Eg: [gist](https://gist.github.com/fahchen/5955661)

    POST /forms/:id/collection

**Parameters**

* `entities` (*Optional* | **array**)


#### Get the collection

Get the collection which posted by the authorized user of a single form

    GET /forms/:id/collection


#### Get the collections

Get the collections of a single form

    GET /forms/:id/collections

