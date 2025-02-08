---
title: Getting Started
description: >-
  getting started with Real Useragent.
author: PyMmdrza
date: 2025-02-08 04:16:06 +0800
categories: [Tutorial]
tags: [getting started, install user agent, useragent, user agent, auto]
pin: false
---

# Real User Agent

## Real User Agent Auto Sync with Requests Method


Generated and Auto Sync User Agent with 'Real UserAgent' Library


---

Auto Sync With Requests Library on Request Header (User-Agent)

```python
import requests
import real_useragent

session = requests.Session()
print(session.headers["User-Agent"])
```
another model with requests library

```python
> req = request.get("https://httpbin.org/user-agent")
> print(req.json()["user-agent"])
```


[nodejs]: https://nodejs.org/
[starter]: https://github.com/real-useragent/getting-started
[pages-workflow-src]: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow
