---
layout: page
title: About
permalink: /about/
weight: 3
---

{% include back-to-top-button.html %}

<div class="row row-cols-2 justify-content-between align-items-center mb-3 mt-5">
    <h1 class="col"><b> About Me </b></h1>
    <div class="col w-auto">
        {% include social.html %}
    </div>
</div>


Hi, I'm **{{ site.author.name }}** :wave:,<br>

I’m a **UX Designer** with a background in **Software Engineering**. My previous experience in **frontend development** and my long-standing interest in how **visual experiences** impact users naturally led me toward UX. Over time, I’ve developed a deep understanding of **UX Design** and how thoughtful design choices enhance user interaction and satisfaction.

I believe my engineering background gives me a **unique perspective on UX**, enabling me to bridge the gap between design and development teams. I bring a collaborative approach that ensures user-centered solutions are both **visually coherent** and **technically feasible**.

<div class="row mt-5 mb-3 gy-4">
{% include about/skills.html title="Design skills" source=site.data.about.ux-skills %}
{% include about/skills.html title="Programming skills" source=site.data.about.programming-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>