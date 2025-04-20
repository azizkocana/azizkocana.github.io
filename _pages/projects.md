---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

<style>
  article p {
    margin-top: 0;
    margin-bottom: 5px;
  }
</style>

{% for project in site.projects %}
  <article>
    <h3>{{ project.title }}</h3>
    <div>
      {{ project.content | markdownify }}
    </div>
  </article>
  <hr>
{% endfor %}