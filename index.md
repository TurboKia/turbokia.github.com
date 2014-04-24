---
layout: page
title: TurboKia
tagline: Supporting tagline
---
{% include JB/setup %}

<h1>Latest Post</h1>
<ul class="posts">
{% for post in site.posts limit:1 %}
<li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
<ul>
<h1>Recent Posts</h1>
<ul class="posts">
{% for post in site.posts offset:1 limit:2 %}
<li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



