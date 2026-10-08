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

I’m a **UX Designer** with a background in **Software Engineering**. I enjoy turning complex problems into simple, intuitive solutions and designing digital products around the needs of their users.

Having worked on both sides of the design–development process, I bring a **technical perspective to UX** and enjoy working closely with developers to create solutions that are **visually coherent** and **technically feasible**.

<div class="row mt-5 mb-3 gy-4">
{% include about/skills.html title="Design skills" source=site.data.about.ux-skills %}
{% include about/skills.html title="Programming skills" source=site.data.about.programming-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>