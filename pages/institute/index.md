---
layout: page
title: Institute
description: Data Science Institute Reichman description
---

# Data Science Institute

Welcome to the {{ site.title }} operating institute pages! Here you can quickly jump to a 
particular page.

<div class="section-index">
  <hr class="panel-line">
  {% for docs_post in site.pages %}
    {% if docs_post.path contains '/institute/' and docs_post.name != 'index.md' %}
      <div class="entry">
        <h5><a href="{{ docs_post.url | prepend: site.baseurl }}">{{ docs_post.title }}</a></h5>
        <p>{{ docs_post.description }}</p>
      </div>
    {% endif %}
  {% endfor %}
  <div class="entry">
    <h5>Visit us at <a href="{{site.other_web_address}}">the Data Science Institute Website</a></h5>
  </div>
</div>
