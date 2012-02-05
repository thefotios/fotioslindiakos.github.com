---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

<p>
Finally almost working on trying to get a blog started.
</p>
<p>
In typical fashion, I am suffering from premature optimization.
I really want this to work, but I have been spending most of my time trying to get the layout perfect. 
But once I am able to focus, this will hopefully be a good thing.
</p>

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
