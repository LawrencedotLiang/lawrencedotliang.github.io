---
title: "Blog"
---

Hello, this is Lawrence, a Master student studying electrical engineering at the University of Queensland, I finished my Bachelor degree in University of New South Wales.<br>
Here will post the work I have done before and also, show some work I'm doing right now.<br>
Hope you guys enjoy it~<br>

---
layout: page
title: Home
---

# Posts

{% for post in site.posts %}
<li>
  <span>{{ post.date | date: "%b %d, %Y" }}</span> &mdash; 
  <a href="{{ post.url }}">{{ post.title }}</a>
</li>
{% endfor %}
