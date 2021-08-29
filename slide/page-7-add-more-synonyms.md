---
title: Add more options for the placeholders

tags:
date: 1007-04-01

layout: layouts/post.njk
---


I've identified phrases/words I might want to change. Now let's add some more options.


```json
{  
    "origin": "#FrontCover# #Page1# #Page2# #Page3#",
    "FrontCover": "Cover page \n---\n\n How-to \"Generate a How-To Zine\" Zine \n\n A WavelengthConf Progzine",
    "Page1": "Page 1 \n---\n\n How-to \n\n write a #bot# \n that makes zines  \n\n  SO THAT YOU CAN \n\n make the #best# \n zine-ziner-zines",
    "Page2": "Page 2 \n---\n\n I have many ideas on \n how to craft a zine, \n\n but struggle with picking \n the #best# phrasing.",
    "Page3": "Page 3 \n---\n\n With a Tracery bot, \n I can generate \n many different #phrasings# \n and pick my #favorite# to draw!",

    "bot": ["bot", "script", "generator", "procedural generator"],
    "best": ["best", "favorite", "fav", "preferred outcome"],
    "favorite": "#best#",
    "phrasings": ["phrasing", "wording", "verbiage"]
}
```