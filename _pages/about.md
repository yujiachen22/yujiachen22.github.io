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

{% if site.show_sections.welcome %}
  {% include_relative includes/welcome.md %}
{% endif %}

{% if site.show_sections.biography %}
  {% include_relative includes/biography.md %}
{% endif %}

{% if site.show_sections.research_interest %}
  {% include_relative includes/research_interest.md %}
{% endif %}

{% if site.show_sections.news %}
  {% include_relative includes/news.md %}
{% endif %}

{% if site.show_sections.publications %}
  {% include_relative includes/publications.md %}
{% endif %}

{% if site.show_sections.research_experience %}
  {% include_relative includes/research_experience.md %}
{% endif %}

{% if site.show_sections.projects %}
  {% include_relative includes/projects.md %}
{% endif %}

{% if site.show_sections.honors_and_rewards %}
  {% include_relative includes/honors_and_rewards.md %}
{% endif %}

{% if site.show_sections.educations %}
  {% include_relative includes/educations.md %}
{% endif %}

{% if site.show_sections.work_experience %}
  {% include_relative includes/work_experience.md %}
{% endif %}

{% if site.show_sections.skills %}
  {% include_relative includes/skills.md %}
{% endif %}

{% include_relative includes/welcome.md %} 

{% include_relative includes/research_interest.md %} 

{% include_relative includes/Working paper.md %} 

{% include_relative includes/Teaching.md %}

{% include_relative includes/biography.md %} 

{% if site.show_sections.updated %}
  {% include_relative includes/updated.md %}
{% endif %}
