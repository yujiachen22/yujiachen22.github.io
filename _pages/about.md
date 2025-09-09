---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

{% if site.show_sections.biography %}
  {% include_relative includes/biography.md %}
{% endif %}

{% if site.show_sections.research_interest %}
  {% include_relative includes/research_interest.md %}
{% endif %}

{% if site.show_sections.educations %}
  {% include_relative includes/educations.md %}
{% endif %}

{% if site.show_sections.working_paper %}
  {% include_relative includes/working_paper.md %}
{% endif %}

{% if site.show_sections.teaching %}
  {% include_relative includes/teaching.md %}
{% endif %}

{% if site.show_sections.updated %}
  {% include_relative includes/updated.md %}
{% endif %}

{% include_relative includes/biography.md %} 

{% include_relative includes/educations.md %}

{% include_relative includes/research_interest.md %} 

{% include_relative includes/working_paper.md %} 

{% include_relative includes/teaching.md %}

{% include_relative includes/updated.md %} 


