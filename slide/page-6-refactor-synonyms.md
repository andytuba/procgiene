---
title: Identify "synonyms" and turn them into placeholders

tags:
date: 1006-04-01

layout: layouts/post.njk
---

We started with a basic grammar that's not really useful.

```json
{  
    "origin": "#FrontCover# #Page1# #Page2# ... #BackCover#",
    "FrontCover": "Cover page\n---\n\nHow-to Zine\n\nA _WavelengthConf_ Progzine Template",
    "Page1": "Page 1\n---\n\nHow-to\n\ndo a thing\n\nSO THAT YOU CAN\n\noutcome of doing the thing.",
    "Page2": "Page 2\n---\n\nDescribe the problem this how-to solves\n\nWhat's the PAIN???"
}
```

What could we replace?

* How-To
* thing
* problem
* pain


```json
{  
    "origin": "#FrontCover# #Page1# #Page2# ... #BackCover#",
    "FrontCover": "Cover page\n---\n\n#How-To# Zine\n\nA _WavelengthConf_ Progzine Template",
    "Page1": "Page 1\n---\n\n#How-to#\n\ndo a #thing#\n\nSO THAT YOU CAN\n\noutcome of doing the #thing#.",
    "Page2": "Page 2\n---\n\nDescribe the #problem# this how-to solves\n\nWhat's the #PAIN#???",

    "How-To": ["How-To"],
    "thing": ["thing"],
    "problem": ["problem"],
    "PAIN": ["PAIN"]
}
```