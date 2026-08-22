---
title: "CV"
layout: gridlay
sitemap: false
permalink: /cv/
---

## Curriculum Vitae

<div class="section-card">
<div class="pi-card">
<div>
<h3 class="pi-name">{{ site.name }}</h3>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if site.links.orcid and site.links.orcid != "" %}<a href="{{ site.links.orcid }}" class="icon-link" title="ORCID"><i class="ai ai-orcid"></i></a>{% endif %}
{% if site.links.linkedin and site.links.linkedin != "" %}<a href="{{ site.links.linkedin }}" class="icon-link" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>{% endif %}
</div>
</div>
</div>
</div>

{% if site.data.pi[0].education %}
<div class="section-card">
<h3>Education</h3>
<ul>
{% for education in site.data.pi[0].education %}
<li>{{ education | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.grants %}
<div class="section-card">
<h3>Research Projects</h3>
<ul>
{% for grant in site.data.grants %}
<li>{{ grant.name }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

<div class="section-card">
<h3>Publications</h3>
{% bibliography %}
</div>

{% if site.data.awards %}
<div class="section-card">
<h3>Awards and Distinctions</h3>
<ul>
{% for award in site.data.awards %}
<li>{{ award.name | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.people %}
<div class="section-card">
<h3>Students Directed (as Principal Advisor)</h3>
<ul>
{% for student in site.data.people %}
<li>{{ student.name }}, {{ student.location }} ({{ student.degree }}, {{ student.year }})</li>
{% endfor %}
</ul>
</div>
{% endif %}

<div class="section-card" markdown="0">
<button onclick="window.print()" style="background: var(--accent-color, #1a7a6d); color: white; border: none; padding: 10px 20px; border-radius: 6px; cursor: pointer; font-size: 0.95rem;">
<i class="fa-solid fa-print"></i> Print / Save as PDF
</button>
</div>
