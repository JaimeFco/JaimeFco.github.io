---
layout: page
title: About
permalink: /about/
weight: 3
---

# **Sobre Mi**

¡Hola! Soy yo, **{{ site.author.name }}** :wave:,<br>
Un día simplemente dije «Vamos a escribir cosas entretenidas», y por eso hice el blog. Otro día empecé a hacer videos en YouTube, pero ese formato no me funcionó. Ahora hago podcast de ciencia. Me gusta el aprendizaje estadístico y las matemáticas.

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>
