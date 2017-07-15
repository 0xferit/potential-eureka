---
layout: default
---

# Blog Posts
{% for post in site.posts %}
## []({{post.url}}){{ post.date | date_to_string }} / {{post.title}}  
  {{post.excerpt}} ... [**More**]({{post.url}})
{% endfor %}
