---
title: What is Tracery?

tags:
date: 1003-01-11

layout: layouts/post.njk
---

Tracery is a software library that _generates text_ given a _grammar_ describing more or less what the text should be.

(That text can be turned into pictures or music or web pages, too--anything that can be described using text.)

## History

Dr Kate Compton, Code Wizard, a.k.a. [@GalaxyKate](https://twitter.com/GalaxyKate), built the Tracery library in 2015 to generate stories from scripts

Now it powers [loads of Twitter bots](https://CheapBotsDoneQuick.com) and builds game dialogue, NPCs, props, and scenery.


## For example,

### A plain English phrase with some placeholders

"We go together like _some nut_ butter and _some fruit_ jelly."

Options for _some nut_:

- peanut
- almond
- avocado nut
- tree nut

Options for _some fruit_:

- strawberry
- raspberry
- avocado
- snozzberry

---

### Tracery grammar representation of that 
```json
{
    "origin": "We go together like #some nut# butter and #some fruit# jelly.",
    "some nut": ["peanut", "almond", "avocado", "tree nut"],
    "some fruit": ["strawberry", "raspberry", "avocado", "snozzberry"]
}
```



### Results [&#x1F517;](http://emptyjug.xxx/tracery/we-go-together)

- We go together like peanut butter and strawberry jelly.
- We go together like almond butter and snozzberry jelly.
- We go together like avocado nut butter and avocado jelly.
