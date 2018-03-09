---
layout: page
title: Записи
permalink: /posts/
backimg: back1.jpg
---
<div class="col-12">
	{% for post in site.posts %}
	    <div class="block-blog">
	        <img src="{{ site.url }}/img/titles/{{ post.mainimg }}" alt="{{ post.title }}" class="img-responsive">
	        <div class="blog-content row">
	            <div class="col-3"><img src="{{ site.url }}/img/logo/{{ post.partnerimg }}" alt="{{ post.title }}" class="img-responsive"></div>
	            <div class="col">
	                <h3>{{ post.title }}</h3>
	                <p>{{ post.description }}</p>
	                <a href="{{ post.url }}" class="btn btn-outline-dark">Читать далее</a>
	            </div>
	        </div>   
	    </div>
	{% endfor %}
</div>


