---
title: Page 7 - Extend the mold - add more synonyms

tags:
date: 1007-01-10

layout: layouts/post.njk
---

Here's where the real magic happens: if I'm not sure I like certain phrasings, I can try mixing it up:

```json
{  
    "origin": "#FrontCover# #Page1# #Page2# ... #BackCover#",
    "FrontCover": "Cover page\n---\n\n**#How-To# Zine**\n\nA _WavelengthConf_ Progzine Template",
    "Page1": "Page 1\n---\n\n**#How-to#**\n\n`do a #thing#`\n\nSO THAT YOU CAN\n\n`outcome of doing the #thing#.`",
    "Page2": "Page 2\n---\n\n`Describe the #problem# this how-to solves`\n\n`What's the #PAIN#???`",

    "How-To": ["How-To", "Guide", "Guidebook"],
    "thing": ["thing", "task", "objective", "assignment"],
    "problem": ["problem", "struggle", "issue", "sticky point"],
    "PAIN": ["PAIN", "#problem#"]
}
```