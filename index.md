---
layout: default
---

{% comment %}
{% for post in site.posts %}
## {{ post.date | date_to_string }} / [{{post.title}}]({{post.url}})  
  {{post.excerpt}} ... [**more**]({{post.url}})
{% endfor %}
{% endcomment %}

{% for post in site.posts %}
{{post.content}}
{% endfor %}
