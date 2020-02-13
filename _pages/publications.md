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

Click on the publication titles to see the abstract and a featured figure!

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
