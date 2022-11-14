---
layout: default
---

<h1 style="text-align:center">Projects</h1>
<br>
{% for project in site.data.projects %}

{% if project.url %}
## [{{ project.name }}]({{ project.url }})
{% else %}
## {{ project.name }}
{% endif %}

{{ project.description }}

{% if project.src %}
[View source]({{ project.src }})
{% endif %}
<hr>
{% endfor %}

{: style="text-align: center"}
See more of my projects on [GitHub](https://github.com/keane-fernandes).