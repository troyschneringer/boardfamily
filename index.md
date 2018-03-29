---
layout: base
---
<header class="justify-center tc bg-blue h3 h5-ns">
	<h1>boardfamily</h1>
</header>
<div class="body-content mt2 mt4-ns">
	<!-- Highlights -->
	<div class="flex-row-ns items-center items-stretch-ns justify-between-ns ph2 ph0-ns">
		{% for post in site.posts limit:3 %}
			{% include game-card.html title=post.title url=post.url date=post.date image=post.image stars=post.stats.stars %}
		{% endfor %}
	</div>
	<!-- /Highlights -->
</div>