---
title: Tracery in Action

tags:
date: 1003-01-12

layout: layouts/post.njk
---

We can write a Tracery _grammar_ which provides the template.

### A quick example 🥪

First, start with a plain sentence:

> "We go together like peanut butter and strawberry jelly.

Now identify parts of the sentence that could be replaced with other words or phrases.

> We go together like ~~peanut~~ _some nut_ butter and ~~strawberry~~ _some fruit_ jelly.

Now that you have a template with placeholders ... 
> We go together like _some nut_ butter and  _some fruit_ jelly.

... what options can go in the placeholders?

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

### Tracery grammar representation of this 🥪 sandwich
Tracery grammars are represented as `{ "json": blobs }`.  
The main template is the `"origin"` value.
The placeholders are marked off with `#hash signs#`.
The options for the placeholders go in the `"placeholder's value"`.

```json
{
    "origin": "We go together like #some nut# butter and #some fruit# jelly.",
    "some nut": ["peanut", "almond", "avocado", "tree nut"],
    "some fruit": ["strawberry", "raspberry", "avocado", "snozzberry"]
}
```

### Potential variations

If we asked a 🤖Tracery engine to flatten that grammar into a final product, we might come out with results like:

- We go together like peanut butter and strawberry jelly.
- We go together like almond butter and snozzberry jelly.
- We go together like avocado nut butter and avocado jelly.

### Demo: [tracery.io editor](http://tracery.io/editor/)

Let's do it live: copy-paste the grammar, then click the "reroll" button.

<iframe src="http://tracery.io/editor/" height="500"></iframe>


### Demo: [emptyjug.xxx/tracery](http://emptyjug.xxx/tracery/we-go-together)

(Click the 🎲 button.)
<iframe src="http://emptyjug.xxx/tracery/we-go-together"></iframe>
