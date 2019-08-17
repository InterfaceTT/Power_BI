---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Click [here](Presentation\ClassLogins.pdf) for access to class information including links and login information for the class.

Click [here](Presentation\PowerBILinks.pdf) for a list of useful books and links on PowerBI.

Below are links to each of the presentation slide decks and lab exercises.

## Presentations

1. [Module 1 Slides](Presentation/20778C_01U.pdf)
2. [Module 2 Slides](Presentation/20778C_02U.pdf)
3. [Module 3 Slides](Presentation/20778C_03U.pdf)
4. [Module 4 Slides](Presentation/20778C_04U.pdf)
5. [Module 5 Slides](Presentation/20778C_05U.pdf)
6. [Module 6 Slides](Presentation/20778C_06U.pdf)
7. [Module 7 Slides](Presentation/20778C_07U.pdf)
8. [Module 8 Slides](Presentation/20778C_08U.pdf)
9. [Module 9 Slides](Presentation/20778C_09U.pdf)

## Labs

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/'" %}
| Module | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}