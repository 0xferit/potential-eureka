---
layout: default
---

# Blog Posts
{% for post in site.posts %}
## [d]({{post.url}}){{ post.date | date_to_string }} / {{post.title}}  
  {{post.excerpt}} ... [**more**]({{post.url}})
{% endfor %}
