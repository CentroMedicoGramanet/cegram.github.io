---
layout: default
title: Galeria
permalink: /fotos/
lightbox: true

---

<main id="page-main" role="main">
	<div id="layout" class="listed">
    	<h3 class="anm-moveFromLeftFade delay-2000"><img src="{{ site.baseurl }}/hipertextos/svg/printer.svg" class="img-icon"><u>Impressions</u></h3>
		<section class="anm-fadeIn delay-2000">					
	{% assign image_files = site.static_files | where: "image", true %}
	{% for image in image_files %}
	<article>
    	<a href="{{ site.baseurl }}/assets/bio/{{ image.name }}" data-lightbox="roadtrip"><img class="imagens" src="{{ site.baseurl }}/assets/bio	/{{ image.name }}" alt="El centro médico"></a>
	</article>
	{% endfor %}
		</section>
	<hr>
	</div><!-- /#Layout -->
</main>
