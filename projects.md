---
layout: page
permalink: /projects/
title: Projects
class: projects
---

# Projects

{:.lead}
These are a select collection of my favorite projects. You can find the code for some of them on [GitHub](https://github.com/frankelavsky). 

{% assign projtypes = site.data.projects | group_by:"type"  %}
{% assign sorted_projtypes = projtypes %}
{% for type in sorted_projtypes %}
<h2 id="{{ type.name | replace: ' ', '-' | replace: '(', '' | replace: ')', '' }}">{{ type.name }}</h2>
<div class="grid">
  <!-- {% for project in site.data.projects %}
    {% include project.html project=project %}
  {% endfor %} -->
  {% for project in type.items %}
  {% include project.html project=project %}
  {% endfor %}
</div>
{% endfor %}

