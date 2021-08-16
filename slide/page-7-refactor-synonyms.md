---
title: Extend the mold - refactor synonyms

tags:
date: 1007-01-01

layout: layouts/post.njk
---


```json
{  
    "origin": "#FrontCover# #Page1# #Page2# ... #BackCover#",
    "FrontCover": "Cover page\n---\n\n**#How-To# Zine**\n\nA _WavelengthConf_ Procgiene Template",
    "Page1": "Page 1\n---\n\n**#How-to#**\n\n`do a #thing#`\n\nSO THAT YOU CAN\n\n`outcome of doing the #thing#.`",
    "Page2": "Page 2\n---\n\n`Describe the #problem# this how-to solves`\n\n`What's the #PAIN#???`",

    "How-To": ["How-To"],
    "thing": ["thing"],
    "problem": ["problem"],
    "PAIN": ["PAIN"]
}
```