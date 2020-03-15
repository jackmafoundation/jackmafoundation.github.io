---
layout: blog-list
title: 新闻动态
permalink: /blog/

header: Latest News
cover: https://img.mayun.xin/upload/2020031416/367fb3c9fc4b86cd1ff9c025f2e34c29.jpg
---

<div class="cbox title-box">
	<ul class="">
	  	{% for post in site.posts %}
			<li class="">
				<span class="publish-date">{{ post.date | date: "%Y-%m-%d" }}</span>
				<a href="{{ post.url }}">{{ post.title }}</a>
			</li>
	  	{% endfor %}
	</ul>
</div>