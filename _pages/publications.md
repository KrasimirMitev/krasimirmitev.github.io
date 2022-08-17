---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

A full list of my publications in pdf format can be downloaded from [here](../files/ListOfPublicartions_KM.pdf){:target="\_blank"}


## Chapters in monographies

{% for post in site.publications reversed %}
{% if post.section == 'ch_mono' %}
{% include archive-single.html %}
{% endif %}
{% endfor %}


## Latest articles in international peer-reviewed journals

{% for post in site.publications reversed %}
{% if post.section == 'peer-rev' %}
{% include archive-single.html %}
{% endif %}
{% endfor %}


## Abstracts and publications in other journals

{% for post in site.publications reversed %}
{% if post.section == 'other' %}
{% include archive-single.html %}
{% endif %}
{% endfor %}


## Latest full text papers in international conference proceedings

{% for post in site.publications reversed %}
{% if post.section == 'conf_proceed' %}
{% include archive-single.html %}
{% endif %}
{% endfor %}


## Latest full text papers in proceedings from national conferences

{% for post in site.publications reversed %}
{% if post.section == 'national_conf' %}
{% include archive-single.html %}
{% endif %}
{% endfor %}

