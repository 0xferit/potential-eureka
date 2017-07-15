---
layout: default
---

# Blog Posts
{% for post in site.posts %}
* {{ post.date | date_to_string }} &#09997; {{post.title}}  
  {{post.excerpt}}
{% endfor %}
