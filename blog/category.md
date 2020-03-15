---
layout: blog-list
title: 文章归档
permalink: /blog/category/

header: Posts filtered by tag
---

{% for tag in site.categories %} 
  <div class="cbox" id="{{ tag[0] }}">
	<div class="box-title">
		<h2>{{ tag[0] | capitalize }}</h2>
    </div>
    <ul class="">
    	{% assign pages_list = tag[1] %} 
	  	{% for post in pages_list %}
			<li class="">
				<span class="publish-date">{{ post.date | date: "%Y-%m-%d" }}</span>
				<a href="{{ post.url }}">{{ post.title }}</a>
			</li>
	  	{% endfor %}
	  	{% assign pages_list = nil %}
	</ul>
  </div>
{% endfor %}