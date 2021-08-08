---
---
{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
{{ post.excerpt }}
##### Posted on {{ post.date | date: "%-d %B %Y" }} by {{ post.author }}
* * *
{% endfor %}