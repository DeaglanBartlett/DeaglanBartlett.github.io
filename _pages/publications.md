---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can also find my articles on my [Google Scholar](https://scholar.google.com/citations?user=wTj4UjSjpBkC&hl=en)
or [arXiv](https://arxiv.org/a/bartlett_d_1.html) profiles.

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
