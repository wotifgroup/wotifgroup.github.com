<div id="popular-tags" class="section">	
	<h2 class="section-title">All Tags</h2>
	<ul>
		{% for tag in site.iterable.tags %}
			<li><a href="/tags/{{ tag.name | replace:' ','-' | downcase }}" name="{{ tag.name | replace:' ','-' | downcase }}">{{ tag.name }}</a></li>
		{% endfor %}
	</ul>
</div>