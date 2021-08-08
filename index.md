---
---
{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
{% capture show_more %}[ [...] ]({{ post.url }}){% endcapture %}
{{ post.excerpt | strip_html | truncate: 200, show_more }}
##### Posted on {{ post.date | date: "%-d %B %Y" }} by {{ post.author }}
* * *
{% endfor %}