---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
<p>
  <a href="{{ post.paperurl }}" target="_blank"><strong>{{ post.title }}</strong></a><br>
  {{ post.authors }}<br>
  <em>{{ post.venue }}</em>
</p>
{% endfor %}
