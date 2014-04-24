---
layout: page
title: TurboKia
tagline: Supporting tagline
---
{% include JB/setup %}

<h1>Latest Post</h1>
{% for post in site.posts limit:1 %}
{% endfor %}
<h1>Recent Posts</h1>
{% for post in site.posts offset:1 limit:2 %}
{% endfor %}

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

This theme is still unfinished. If you'd like to be added as a contributor, [please fork](http://github.com/plusjade/jekyll-bootstrap)!
We need to clean up the themes, make theme usage guides with theme-specific markup examples.


