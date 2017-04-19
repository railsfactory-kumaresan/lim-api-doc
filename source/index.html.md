---
title: API Reference

language_tabs:
  - shell

toc_footers:
  - <a href='#'>Documentation Powered by LIM</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the LIM API! You can use our API to access LIM API endpoints, which can get information on saved URLs and to save the url content(a, h1, h2, h3)

# URL Crawler

## Save URL contents

```shell
curl "http://api.lim.com/v1/crawler_urls"
```
> Example Request JSON:

```json
  {
    "url": "https://testurl.com"
  }
```

> Example Success Response JSON:

```json
  {
    "url": "https://testurl.com",
    "content":{
      "a":["http://emberjs.com/", "http://emberjs.com/"],
      "h1":["Building a Simple Component\n Edit Page"],
      "h2":["Hiding and Showing an Image"],
      "h3":[]
    }
  }
```

This endpoint save the page contents.

### HTTP Request

`POST http://api.lim.com/v1/crawler_urls`

### Request Body Parameters

Parameter | Type | Description
--------- | ------- | -----------
url*    | string | URL of the saved content


### Errors

Message    | Description
---------- | ----------------
Url can't be blank | If the given url is blank.
Url must be a valid URL | If the given url not match the url pattern.

## Get all the saved URLs


```shell
curl "http://api.lim.com/v1/crawler_urls"
```

> Example Response JSON:

```json
  [
    "http://gutmann.info",
    "http://ratkebotsford.ca",
    "http://fritsch.us",
    "http://klocko.us"
  ]
```

This endpoint fetch all the saved urls from the system.


### HTTP Request

`GET http://api.lim.com/v1/crawler_urls`