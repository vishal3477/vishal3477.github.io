---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  You can also find my articles on <a href="{{ site.author.googlescholar }}">Google Scholar</a>.
{% endif %}

{% include base_path %}

Published papers, accepted work, and preprints are listed together by year, newest first. Preprints and workshop acceptances are labeled on each card.

{% assign publications = site.publications | sort: 'date' | reverse %}
{% assign publication_years = publications | group_by_exp: 'post', "post.date | date: '%Y'" %}
{% for year in publication_years %}
<section class="publication-year-group" aria-labelledby="publications-{{ year.name }}">
  <h2 id="publications-{{ year.name }}">{{ year.name }}</h2>
  <div class="publication-list">
  {% for post in year.items %}
    {% include publication-card.html %}
  {% endfor %}
  </div>
</section>
{% endfor %}
