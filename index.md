---
layout: page
title: PDXScala
tagline: Scala is alive in lovely Portland, Oregon
---
{% include JB/setup %}

<div id="home">
	{% for post in site.posts limit:5 %}
	<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
	<div class="post">
		{{ post.content }}
		<div class="item_meta">
			<span class="posted_on">
				Posted on <a href="{{ post.url }}">{{ post.date | date_to_string }}</a>
			</span>
		</div>
	</div>
	<br/>
	{% endfor %}
</div>
