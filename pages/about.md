---
layout: page
title: About
permalink: /about/
weight: 3
---

# **Sobre Mi**

¡Hola! Soy yo, **{{ site.author.name }}** :wave:,<br>
No estoy seguro qué escribir aquí.

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>
