---
title: Add more options for the placeholders

tags:
date: 1006-04-01

layout: layouts/post.njk
---

Almost there! Now that I've identified phrases I might want to change, like "how-to" and "thing", I can add in more options for synonyms.

```json
{  
    "origin": "#FrontCover# #Page1# #Page2# ... #BackCover#",
    "FrontCover": "Cover page \n---\n\n #How-To# Zine \n\n A _WavelengthConf_ Progzine Template",
    "Page1": "Page 1 \n---\n\n #How-to# \n\n do a #thing# \n\n SO THAT YOU CAN \n\n outcome of doing the #thing#.",
    "Page2": "Page 2 \n---\n\n Describe the #problem# this how-to solves \n\n What's the #PAIN#???",

    "How-To": ["How-To", "Guide", "Guidebook"],
    "thing": ["thing", "task", "objective", "assignment"],
    "problem": ["problem", "struggle", "issue", "sticky point"],
    "PAIN": ["PAIN", "#problem#"]
}
```