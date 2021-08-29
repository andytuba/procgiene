---
title: Generate variations

tags:
date: 1006-05-01

layout: layouts/post.njk
---

Now that we have a versatile template, let's generate some variations.

Find a Tracery engine, feed it your grammar, and [see what 🤖tracery generates](http://emptyjug.xxx/tracery/progzine-how-to-template):

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

What will this grammar result in? (FYI, I tagged the `#synonyms#` with 🤖 to make it easier to identify what changed.)

<iframe src="http://emptyjug.xxx/tracery/progzine-how-to-template" />
