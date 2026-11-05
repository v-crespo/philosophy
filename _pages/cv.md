---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<!-- Put your CV in the "files" folder with exactly this name: cv.pdf -->
**[Download my full CV (PDF)]({{ base_path }}/files/cv.pdf)** · Last updated [MONTH YEAR]

Education
======
* Ph.D. in Philosophy, Duke University, [YEAR] (expected)
  * Dissertation: *[DISSERTATION TITLE]*
  * Committee: [ADVISOR NAME] (chair), [MEMBER NAME], [MEMBER NAME]
* [DEGREE, e.g. M.A. in Philosophy], [UNIVERSITY], [YEAR]
* [DEGREE, e.g. B.A. in Philosophy], [UNIVERSITY], [YEAR]

Areas
======
* **Specialization:** Philosophy of AI, Ethics
* **Competence:** PPE, Decision Theory

Research
======
<!-- This list fills in automatically from the papers in the _publications folder. -->
{% for category in site.publication_category %}
  {% assign papers = site.publications | where: "category", category[0] | reverse %}
  {% if papers.size > 0 %}
  <h3>{{ category[1].title }}</h3>
  <ul>{% for post in papers %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  {% endif %}
{% endfor %}

Talks and Commentaries
======
<!-- This list fills in automatically from the _talks folder. -->
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>

Teaching
======
<!-- This list fills in automatically from the _teaching folder. -->
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Awards and Fellowships
======
* [NAME OF AWARD OR FELLOWSHIP], [INSTITUTION], [YEAR]
* [NAME OF AWARD OR FELLOWSHIP], [INSTITUTION], [YEAR]

Service
======
* Referee for [JOURNAL NAME]
* [ROLE, e.g. Organizer], [EVENT OR WORKSHOP], [YEAR]
* [ROLE, e.g. Graduate Student Representative], Duke University Department of Philosophy, [YEARS]

Languages
======
* [LANGUAGE] ([native / fluent / reading knowledge])
* [LANGUAGE] ([native / fluent / reading knowledge])

References
======
* [REFEREE NAME], [TITLE], [UNIVERSITY], [EMAIL]
* [REFEREE NAME], [TITLE], [UNIVERSITY], [EMAIL]
* [REFEREE NAME], [TITLE], [UNIVERSITY], [EMAIL]
* [REFEREE NAME] (teaching), [TITLE], [UNIVERSITY], [EMAIL]
