---
title: "CV"
layout: gridlay
sitemap: false
permalink: /cv/
---

<style>
.cv-header { text-align: center; margin-bottom: 2rem; }
.cv-header h2 { margin-bottom: 0.25rem; }
.cv-header p { color: var(--text-secondary); font-style: italic; }
.cv-print-btn { display: inline-block; margin-top: 1rem; background: var(--accent-color, #1a7a6d); color: white; border: none; padding: 8px 18px; border-radius: 6px; cursor: pointer; font-size: 0.9rem; text-decoration: none; }
.cv-section-title { font-size: 1.3rem; font-weight: 700; margin: 2.5rem 0 1rem 0; border-bottom: 2px solid var(--accent-color, #1a7a6d); padding-bottom: 0.4rem; }
.cv-timeline { border-left: 2px solid rgba(26,122,109,0.3); margin-left: 0.5rem; padding-left: 1.5rem; }
.cv-entry { position: relative; margin-bottom: 1.6rem; }
.cv-entry::before { content: ""; position: absolute; left: -1.85rem; top: 0.3rem; width: 10px; height: 10px; border-radius: 50%; background: var(--accent-color, #1a7a6d); }
.cv-date { font-size: 0.85rem; color: var(--text-secondary); font-weight: 600; letter-spacing: 0.02em; }
.cv-title { font-weight: 700; font-size: 1.05rem; margin: 0.15rem 0 0 0; }
.cv-subtitle { font-style: italic; color: var(--text-secondary); margin: 0 0 0.4rem 0; font-size: 0.95rem; }
.cv-desc { font-size: 0.95rem; line-height: 1.5; }
.cv-desc ul { margin-top: 0.4rem; }
</style>

<div class="cv-header">
<h2>{{ site.name }}</h2>
<p>{{ site.title }}, {{ site.institution }}</p>
<a class="cv-print-btn" onclick="window.print()"><i class="fa-solid fa-print"></i> Print / Save as PDF</a>
</div>

<div class="cv-section-title">Professional Summary</div>
<p>Geologist and geophysicist working at the intersection of inverse theory, compressive sensing, and deep learning applied to geophysical exploration. Currently completing a PhD in Computer Science at Universidad Industrial de Santander, with research focused on 3D survey geometry optimization and recovery algorithms for compressive seismic acquisition.</p>

<div class="cv-section-title">Experience</div>
<div class="cv-timeline">
<div class="cv-entry">
<div class="cv-date">Aug 2025 – Present</div>
<div class="cv-title">Researcher & Lecturer</div>
<div class="cv-subtitle">Universidad Industrial de Santander</div>
<div class="cv-desc">Teaching "Fundamentos de Geofísica I" (graduate level). Co-investigator, Contract 045-2025 UIS-MINCIENCIAS on joint inversion of gravimetry, magnetometry, and magnetotelluric data for geothermal exploration at Cerro Machín volcano.</div>
</div>
<div class="cv-entry">
<div class="cv-date">Jan 2024 – Aug 2025</div>
<div class="cv-title">Co-investigator</div>
<div class="cv-subtitle">Universidad Industrial de Santander — Project 3925</div>
<div class="cv-desc">Improvement of seismic imaging in emerging Colombian basins.</div>
</div>
<div class="cv-entry">
<div class="cv-date">Sep 2023 – Dec 2023</div>
<div class="cv-title">Visiting Research Intern</div>
<div class="cv-subtitle">Washington University in St. Louis — Computational Imaging Group</div>
<div class="cv-desc">Research internship funded by UIS and Washington University in St. Louis. Advanced applications of deep learning in geophysical problems, focused on diffusion models for seismic data reconstruction.</div>
</div>
<div class="cv-entry">
<div class="cv-date">Nov 2021 – Sep 2023</div>
<div class="cv-title">Program Coordinator & Lecturer</div>
<div class="cv-subtitle">Universidad Industrial de Santander</div>
<div class="cv-desc">Coordinated talent development for MSc Geophysics research-internship students. Taught "Fundamentos de Geofísica II" and "Introducción a la Sismología." Co-investigator, Project 9836 (MINCIENCIAS & ANH) on 3D seismic acquisition geometry design.</div>
</div>
<div class="cv-entry">
<div class="cv-date">Jun 2019 – Sep 2021</div>
<div class="cv-title">Research Professional</div>
<div class="cv-subtitle">Universidad Industrial de Santander</div>
<div class="cv-desc">Deep learning applied to seismic data design and processing in frontier basins.</div>
</div>
<div class="cv-entry">
<div class="cv-date">Oct 2018 – May 2019</div>
<div class="cv-title">Director, R&D Unit</div>
<div class="cv-subtitle">INGEOSUR SAS</div>
<div class="cv-desc">Founded and directed the Computational Geosciences R&D Unit. Designed AI-based methodologies for geophysics and environmental geology.</div>
</div>
</div>

<div class="cv-section-title">Education</div>
<div class="cv-timeline">
<div class="cv-entry">
<div class="cv-date">2019 – Present</div>
<div class="cv-title">Ph.D. Computer Science</div>
<div class="cv-subtitle">Universidad Industrial de Santander</div>
<div class="cv-desc">Optimization of 3D Survey Geometry and Recovery Algorithm in Compressive Seismic Acquisition.</div>
</div>
<div class="cv-entry">
<div class="cv-date">2016 – 2018</div>
<div class="cv-title">M.Sc. Geology/Geophysics</div>
<div class="cv-subtitle">Perm State University, Russia</div>
<div class="cv-desc">Pre-stack seismic migration applied to karst cave detection in the Ural region.</div>
</div>
<div class="cv-entry">
<div class="cv-date">2015 – 2016</div>
<div class="cv-title">Specialization, Environmental Geotechnics</div>
<div class="cv-subtitle">Universidad de Santander</div>
</div>
<div class="cv-entry">
<div class="cv-date">2009 – 2014</div>
<div class="cv-title">B.S. Geology</div>
<div class="cv-subtitle">Universidad Industrial de Santander</div>
<div class="cv-desc">Study of dynamic topography effects on the Nazca Plate.</div>
</div>
</div>

<div class="cv-section-title">Awards & Distinctions</div>
<div class="cv-timeline">
{% for award in site.data.awards %}
<div class="cv-entry">
<div class="cv-title">{{ award.name | replace: "-","&#8211;" }}</div>
</div>
{% endfor %}
</div>

<div class="cv-section-title">Research Interests</div>
<p>Inverse Theory & Applications in Geophysics · Artificial Intelligence · Environmental Geology · Applied and Computational Geophysics</p>

<div class="cv-section-title">Languages</div>
<p><strong>Spanish:</strong> Native · <strong>English:</strong> Professional working proficiency · <strong>Russian:</strong> Professional working proficiency</p>

<div class="cv-section-title">Selected Publications</div>
{% bibliography %}
</div>
