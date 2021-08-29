---
title: Convert it into a Tracery grammar

tags:
date: 1006-02-01

layout: layouts/post.njk
---

We just looked at the text of that "final draft". Next step is to convert it into a Tracery grammar, which is a straightforward JSON blob:

```json
{  
    "origin": "#FrontCover# \n\n #Page1# \n\n #Page2# \n\n ... \n\n #BackCover#",
    "FrontCover": "Cover page \n---\n\n How-to Zine \n\n A WavelengthConf Progzine Template",
    "Page1": "Page 1 \n---\n\n How-to \n\n do a thing \n\n SO THAT YOU CAN \n\n `outcome of doing the thing.",
    "Page2": "Page 2 \n---\n\n Describe the problem this how-to solves \n\n What's the PAIN???"
}
```

The JSON blob above is a Tracery grammar, representing the plain text below.

---

## Page 1
**How-to**

`do a thing`

SO THAT YOU CAN

`outcome of doing the thing.`

## Page 2

`Describe the problem this how-to solves.`

`What's the PAIN???`
