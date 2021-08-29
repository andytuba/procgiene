---
title: Identify "synonyms" and turn them into placeholders

tags:
date: 1007-04-01

layout: layouts/post.njk
---

Again, we started with a basic grammar that's not really useful. What could we replace?

* bot
* best
* favorites
* phrasing


```json
{  
    "origin": "#FrontCover# #Page1# #Page2# #Page3#",
    "FrontCover": "Cover page \n---\n\n How-to \"Generate a How-To Zine\" Zine \n\n A WavelengthConf Progzine",
    "Page1": "Page 1 \n---\n\n How-to \n\n write a #bot# \n that makes zines  \n\n  SO THAT YOU CAN \n\n make the #best# \n zine-ziner-zines",
    "Page2": "Page 2 \n---\n\n I have many ideas on \n how to craft a zine, \n\n but struggle with picking \n the #best# phrasing.",
    "Page3": "Page 3 \n---\n\n With a Tracery bot, \n I can generate \n many different #phrasings# \n and pick my #best# to draw!",

    "bot": ["bot"],
    "best": ["best", "favorite"],
    "phrasings": ["phrasing"]
}
```