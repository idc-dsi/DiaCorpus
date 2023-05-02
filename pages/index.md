---
layout: page
description: Pages index page
---

# Pages

Welcome to the {{ site.title }} pages page! Here you can quickly jump to a 
particular page.


<div class="section-index">
  <hr class="panel-line">
  {% for docs_post in site.pages %}
    {% if docs_post.title != 'index' %}
      <div class="entry">
        <h5><a href="{{ docs_post.url | prepend: site.baseurl }}">{{ docs_post.title }}</a></h5>
        <p>{{ docs_post.description }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>