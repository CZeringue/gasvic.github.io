---
layout: main
---
# Show history

History is available for the following shows:
{% for pg in site.pages %}
{% if pg.url contains "/shows/" %}
* [{{ post.date | date: "%b %Y" }} {{post.title}}]({{post.url}})
{% endif %}
{% endfor %}