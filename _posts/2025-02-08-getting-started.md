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
- UserAgent

```python
from real_useragent import UserAgent
ua = UserAgent()
random_useragent = ua.random_useragent()
```

### Random User Agent from Browser Name:

```python
from real_useragent import UserAgent
ua = UserAgent()
chrome_useragent = ua.chrome_useragent()
firefox_useragent = ua.firefox_useragent()
desktop_useragent = ua.desktop_useragent()
mobile_useragent = ua.mobile_useragent()
safari_useragent = ua.safari_useragent()
```

### Random User Agent from Device Type and Browser :

```python
from real_useragent import UserAgent
ua = UserAgent()
mobile_firefox_ua = ua.get_useragent(mode="mobile", browser="firefox")
desktop_chrome_ua = ua.get_useragent(mode="desktop", browser="chrome")
```
### Random User Agent for Device Type (`mode`)

```python
from real_useragent import UserAgent
ua = UserAgent()
# mode : [desktop or mobile]
desktop_useragent = ua.get_useragent(mode="desktop")
mobile_useragent = ua.get_useragent(mode="mobile")
```
- Desktop

```python
from real_useragent import UserAgent
ua = UserAgent()
desktop_firefox_useragent = ua.desktop_firefox_useragent()
desktop_chrome_useragent = ua.desktop_chrome_useragent()
desktop_linux_useragent = ua.desktop_linux_useragent()
desktop_mac_useragent = ua.desktop_mac_useragent()
```

- Mobile :

```python
from real_useragent import UserAgent
ua = UserAgent()
mobile_chrome_useragent = ua.mobile_chrome_useragent()
mobile_firefox_useragent = ua.mobile_firefox_useragent()
mobile_safari_useragent = ua.mobile_safari_useragent()
```


User Agents are Randomized Per-Session or Per-Request. Individual HTTP requests without a session will each have a random User-Agent selected from the list in [desktop_useragent.txt](https://github.com/UserAgenter/real-useragent/blob/main/real-useragent/desktop_useragent.txt) or [mobile_useragent.txt](https://github.com/UserAgenter/real-useragent/blob/main/real-useragent/mobile_useragent.txt) all files automatically updated every 8 hours.


---

# Donate

Donate with Bitcoin: `1MMDRZA12xdBLD1P5AfEfvEMErp588vmF9`


[nodejs]: https://nodejs.org/
[starter]: https://github.com/real-useragent/getting-started
[pages-workflow-src]: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow
