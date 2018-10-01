---
permalink: /dojos/
layout: page_no_title
---

<header>
	<h1 class="h0 py-4 mt-3">Coding Dojos</h1>
</header>
<div class="col-4 sm-width-full border-top-thin"></div>

<div class="container mx-auto px-2 py-4">
	{% for category in site.categories %}
		{% if category[0] == 'dojos' %}
			{% for post in category[1] %}
				{% include post_block.html %}
			{% endfor %}
		{% endif %}
	{% endfor %}
</div>