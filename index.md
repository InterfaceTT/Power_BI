---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Hyperlinks to each of the presentation slides, lab exercises and demo instructions are listed below.

## Presentations

1. [Module 1 Slides]
2. [Module 2 Slides](Presentation/20778C_02U.pdf)
3. [Module 3 Slides]
4. [Module 4 Slides]
5. [Module 5 Slides]
6. [Module 6 Slides]
7. [Module 7 Slides]
8. [Module 8 SLides]

## Labs

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/'" %}
| Module | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}