---
title: Random User Agent from Browser Name
description: >-
  Generated random real user agent on python with real-useragent library.
author: PyMmdrza
date: 2025-02-07 05:43:16 +0800
categories: [Tutorial, browser]
tags: [python, user agent, web scraping, automation, testing, chrome, library, development]
pin: false
---

## Random User Agent from Browser Name

Generated random real user agent on python with real-useragent library

```python
from real_useragent import UserAgent
ua = UserAgent()
mobile_firefox_ua = ua.get_useragent(mode="mobile", browser="firefox")
desktop_chrome_ua = ua.get_useragent(mode="desktop", browser="chrome")
```

---

[generate-android-useragent]: https://github.com/useragenter/generate-android-useragent


