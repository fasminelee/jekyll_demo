---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home

# layout: default
title: 我的Blog
---

<h2>{{ page.title }}</h2>

<p>最新文章</p>

<ul>

	{% for post in site.posts %}

	<li>{{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>

	{% endfor %}

</ul>



