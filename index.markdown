---
layout: home
title: WotifGroup Technical Blog
---

Welcome to the <a href="http://wotifgroup.github.com/">WotifGroup Technical Blog</a>.

Brought to you by all the teams keeping the site(s) running...

<div id="blog-posts">
	{% for post in site.posts limit: 5 %}
	<div class="post{% if forloop.first %} first{% endif %}">
		<h1 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h1>
		<div class="post-meta">
			<span class="date"><img src="/images/icons/ico_calendar.png" alt="" />{{ post.date | date_to_string }} | </span>
			<span class="categories">
				<img src="/images/icons/ico_drawer.png" alt="" />
				Tags: {% for tag in post.tags limit: 3 %}<a href="/tags/{{ tag | replace:' ', '-' | downcase }}">{{ tag }}{% if forloop.last == false %}, {%endif %}</a> {% endfor %}
			</span>
		</div>
		{{ post.content | markdownify | html_truncatewords }} <a class="more-link" href="{{ post.url }}">Read More&hellip;</a>
	</div><!-- end: .post -->
	{% endfor %}
</div>


