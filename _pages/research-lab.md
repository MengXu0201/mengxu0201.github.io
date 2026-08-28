---
layout: archive
title: "Research Lab"
permalink: /research-lab/
author_profile: true
research_areas:
  - Medical Image Analysis
  - Breast Cancer Risk Prediction
  - Medical Video Understanding
  - Trustworthy & Efficient AI
  - Quantum Machine Learning
projects:
  - title: Breast Cancer Risk Prediction from Longitudinal Mammograms
  - title: AI for Medical Ultrasound and Video Analysis
  - title: Quantum Machine Learning for Medical Imaging
  - title: Robust and Trustworthy Medical AI
team:
  - group: Faculty
    members:
      - name: Meng Xu, Ph.D.
        role: Assistant Professor
        affiliation:
          - Department of Computer Science and Technology
          - Kean University
  - group: Graduate Students
    members:
      - name: Skyler LaFisca
      - name: Gustavo Garcia Vargas
  - group: Undergraduate Researchers
    members:
      - name: Madeline Jewett
      - name: Allen Ramirez
  - group: Lab Alumni
    members:
      - name: Rayleen Ramos
        links:
          - label: See her work
            url: https://youtu.be/Heqgo00UEgM?si=atyGRgcKtOjDCDgV
      - name: Cesar Marte Jimenez
---

{% include base_path %}

## About the Lab

Our research focuses on artificial intelligence, computer vision, medical imaging, and emerging quantum machine learning methods. We are particularly interested in developing practical and trustworthy AI methods for biomedical and healthcare applications.

## Research Areas

<ul>
{% for area in page.research_areas %}
  <li>{{ area | escape }}</li>
{% endfor %}
</ul>

## Current Research Projects

<!--
Optional project fields supported below:
description, image, publication_url, github_url, website_url.
Only fields that exist will be displayed.
-->

{% for project in page.projects %}
  <div class="list__item">
    <article class="archive__item">
      <h3 class="archive__item-title">{{ project.title | escape }}</h3>

      {% if project.description %}
        <p class="archive__item-excerpt">{{ project.description | escape }}</p>
      {% endif %}

      {% if project.image %}
        <p><img src="{% if project.image contains '://' %}{{ project.image }}{% else %}{{ project.image | relative_url }}{% endif %}" alt="{{ project.title | escape }}"></p>
      {% endif %}

      {% if project.publication_url or project.github_url or project.website_url %}
        <p>
          {% if project.publication_url %}
            <a href="{{ project.publication_url }}">Publication</a>{% if project.github_url or project.website_url %} | {% endif %}
          {% endif %}
          {% if project.github_url %}
            <a href="{{ project.github_url }}">GitHub</a>{% if project.website_url %} | {% endif %}
          {% endif %}
          {% if project.website_url %}
            <a href="{{ project.website_url }}">Project Website</a>
          {% endif %}
        </p>
      {% endif %}
    </article>
  </div>
{% endfor %}

## Research Team

<!--
Optional member fields supported below:
photo, role, affiliation, degree, research_interests, website_url, linkedin_url, github_url, links.
Only fields that exist will be displayed.
-->

{% for team_group in page.team %}
### {{ team_group.group }}

{% for member in team_group.members %}
  <div class="list__item">
    <article class="archive__item">
      {% if member.photo %}
        <p><img src="{% if member.photo contains '://' %}{{ member.photo }}{% else %}{{ member.photo | relative_url }}{% endif %}" alt="{{ member.name | escape }}"></p>
      {% endif %}

      <p><strong>{{ member.name | escape }}</strong>{% if member.role %}<br>{{ member.role | escape }}{% endif %}{% if member.degree %}<br>{{ member.degree | escape }}{% endif %}{% if member.affiliation %}{% for line in member.affiliation %}<br>{{ line | escape }}{% endfor %}{% endif %}{% if member.research_interests %}<br>{{ member.research_interests | escape }}{% endif %}</p>

      {% if member.website_url or member.linkedin_url or member.github_url or member.links %}
        <p>
          {% if member.website_url %}
            <a href="{{ member.website_url }}">Website</a>{% if member.linkedin_url or member.github_url or member.links %} | {% endif %}
          {% endif %}
          {% if member.linkedin_url %}
            <a href="{{ member.linkedin_url }}">LinkedIn</a>{% if member.github_url or member.links %} | {% endif %}
          {% endif %}
          {% if member.github_url %}
            <a href="{{ member.github_url }}">GitHub</a>{% if member.links %} | {% endif %}
          {% endif %}
          {% for link in member.links %}
            <a href="{{ link.url }}" target="_blank" rel="noopener noreferrer">{{ link.label }}</a>{% unless forloop.last %} | {% endunless %}
          {% endfor %}
        </p>
      {% endif %}
    </article>
  </div>
{% endfor %}
{% endfor %}

## Research Opportunities

My research team is always looking for self-motivated undergraduate and graduate students interested in joining our projects. Please feel free to contact me directly about volunteer or, when available, paid research opportunities.

**Undergraduate students:** Should have completed or be currently taking a Data Structures course.

**Graduate students:** No specific course prerequisites are required.

**Requirements for all students:** Strong coding skills, high self-motivation, and a genuine eagerness to learn.

Prospective M.S. and Ph.D. students interested in joining my research group are also welcome to contact me. Please email your CV and a brief description of your research interests to <a href="mailto:meng.xu@kean.edu">meng.xu@kean.edu</a>.
