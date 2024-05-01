---
layout: page
permalink: /publications/
title: Publications
description: 
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->


{% if site.scholar.enable_publication_thumbnails %}
<div class="publications">
	{% bibliography -f {{ site.scholar.bibliography }} --group_by none --query @*[selected=true]* %}
</div>
{% else %}
<div class="publications">
	{% bibliography -f {{ site.scholar.bibliography }} %}
</div>
{% endif %}
