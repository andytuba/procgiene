---
layout: layouts/post.njk
title: about
templateClass: tmpl-post
eleventyNavigation:
  key: about
  order: 3
---

<div class="flex-two-column flex-centered">
<img 
  src="{{'/img/andytuba-by-tsunamino-20200126.jpg' | url }}" 
  alt="Headshot of andytuba, photographed by @tsunamino, Jan 2020" 
  class="avatar"
  style="
  height: 150px;
  width: 150px;
">
<div>
<blockquote style="margin-inline-start: 1em;">
Many moons ago my papa took a hard corner in her Beetle and a loose piece of condensed milk flew out of a glove box and pegged me in my skull. I pretend that's when I got my impeccable sense of humor. <a href="http://emptyjug.xxx/tracery/speaker-bio/">⛲</a>
</blockquote>

<p>– <a href="{{ metadata.author.url | url }}">{{ metadata.author.name }} </a></p>
</div>