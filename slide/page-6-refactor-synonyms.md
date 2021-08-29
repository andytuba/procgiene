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
    "FrontCover": "Cover page \n---\n\n How-to Zine \n\n A _WavelengthConf_ Progzine Template",
    "Page1": "Page 1 \n---\n\n How-to \n\n do a thing \n\n SO THAT YOU CAN \n\n outcome of doing the thing.",
    "Page2": "Page 2 \n---\n\n Describe the problem this how-to solves \n\n What's the PAIN???"
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
    "FrontCover": "Cover page \n---\n\n #How-To# Zine \n\n A _WavelengthConf_ Progzine Template",
    "Page1": "Page 1 \n---\n\n #How-to# \n\n do a #thing# \n\n SO THAT YOU CAN \n\n outcome of doing the #thing#.",
    "Page2": "Page 2 \n---\n\n Describe the #problem# this how-to solves \n\n What's the #PAIN#???",

    "How-To": ["How-To"],
    "thing": ["thing"],
    "problem": ["problem"],
    "PAIN": ["PAIN"]
}
```