---
layout: default
---

# Welcome to the Adelaide Bioinformatics workshop programme!

<br>

## Latests posts

{% assign post = site.posts.first %}

<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{ post.date | date_to_string }}</p>
<p>{{ post.excerpt }} ...</p>

<br>


## Recent posts

{% for post in site.posts offset:1 limit:3 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.date | date_to_string }}</p>
  <p>{{ post.excerpt }} ...</p>
{% endfor %}

<br>

### [All posts...](/archive/)
