---
title: Convert it into a Tracery grammar

tags:
date: 1006-01-20

layout: layouts/post.njk
---

Here's the Tracery grammar:

```json
{  
    "origin": "#FrontCover# #Page1# #Page2# ... #BackCover#",
    "FrontCover": "Cover page \n---\n\n How-to Zine \n\n A WavelengthConf Progzine Template",
    "Page1": "Page 1 \n---\n\n How-to \n\n do a thing \n\n SO THAT YOU CAN \n\n `outcome of doing the thing.",
    "Page2": "Page 2 \n---\n\n Describe the problem this how-to solves \n\n What's the PAIN???"
}
```

The above JSON blob is a Tracery grammar, representing the plain text below.

---

## Page 1
**How-to**

`do a thing`

SO THAT YOU CAN

`outcome of doing the thing.`

## Page 2

`Describe the problem this how-to solves.`

`What's the PAIN???`
