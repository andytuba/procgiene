---
title: Is it good enough to ship?
description: 
date: 2021-08-01
tags:
  - flush the buffer
  - satisfice
  
layout: layouts/post.njk
---

## Philosophy and Tactics

### Am I spinning in circles?

If I'm struggling to decide "is this good enough," I have some quick rubrics:

- does it have a low "blast radius"
- what's my escape hatch(es)
- does it meet the team's rubric for quality?

### Don't boil the ocean

Keep eyes on the prize! If there's opportunities to raise the quality in aspects that aren't directly related
to what I'm trying to accomplish, I can take those on ... _after_ I accomplish my main goal.



## Sociotechnical Tooling

### Reduce the blast radius

Did I set up a mechanism to prevent this from impacting people outside the scope I want? Not just end users but co-workers who have to fix the problem!

Feature flags are friends.

### Escape hatches

If this turns out bad, how do I easily recover?

### Rubrics: What's the bar for "quality?"

If I'm working on a team, we should agree on a rubric for "good enough". Ain't nobody got time to
constantly re-litigate quality standards, so write them down -- preferably in a machine-readable format
that you can feed into automated tooling like linters.



### Linters

Can the computer enforce the quality standards?

- The linter can warn "this bit doesn't match the desired style!"
- The linter can probably automatically fix issues.
- The linter _should_ only touch what I actively worked on, so I'm not drawn into boiling the ocean.
