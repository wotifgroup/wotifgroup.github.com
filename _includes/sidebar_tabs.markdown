<div id="side-tabs"> 
	<ul class="tabnav clearfix">
		<li class="active"><a href="#ui-tabs-1">Recent</a></li>
		<li><a href="#ui-tabs-2">Categories</a></li>
	</ul>
	<div id="ui-tabs-1" class="tab-content">
		<ul>
			{% for post in site.posts limit: 5 %}
				<li><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
			{% endfor %}
		</ul>
	</div>
	<div id="ui-tabs-2" class="tab-content">
		<ul>
			{% for topic in site.iterable.categories %}
				<li><a href="/categories/{{ topic.name }}">{{ topic.name }}</a></li>
			{% endfor %}
		</ul>
	</div>
</div>
