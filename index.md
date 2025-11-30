---
layout: home
title: Home
---

<div id="intro-wrapper" class="l-text">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="/images/portrait.jpg"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Hi, I'm Grace C. Kim</h1>
			<div id="intro-subtitle">CS BS/MS Student at Georgia Tech</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<!-- <hr class="l-middle home-hr"> -->
	<div id="everything-else" class="l-middle">
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<a href="{{ site.url }}/cv/#publications"><div><i class="fa fa-list-ul icon icon-right-space"></i>Publications</div></a>
	</div>
	<div>
		My research focuses on improving the <b>interpretability</b> and <b>trustworthiness</b> of ML models. I develop <b>interactive visualization tools</b> for visually analyzing model decision-making, and <b>interpretability methods</b> for understanding and controlling model behavior.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I am pursuing the 4-year BS/MS program at Georgia Tech, working with <a href="http://www.cc.gatech.edu/~dchau/">Polo Chau</a> and <a href="https://eilab.gatech.edu/mark-riedl.html">Mark Riedl</a>. I am fortunate to be supported by the <a href="https://stampsps.gatech.edu/">Stamps President’s Scholarship</a>.
	</div>
	<!-- <div style="height: 1rem"></div>
	<div>
		I have collaborated with designers, developers, artists, and scientists while working at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/apple.svg"> Apple, <img class="intro-logo" style="width: 18px; padding-bottom: 3px;" src="/images/microsoft.svg"> Microsoft Research, <img class="intro-logo" style="width: 24px" src="/images/nasa.svg"> NASA Jet Propulsion Lab, and <img class="intro-logo" style="width: 24px;" src="/images/pnnl.svg"> Pacific Northwest National Lab.
	</div> -->
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title">Featured <a href="/cv/#publications">Research Publications</a></h2>

<!-- <p class="feature-text">
	Latest research for fans of human-computer interaction, data visualization, and machine learning.
</p> -->

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

{% comment %}
<br>
<h2 class="feature-title">Apple <a href="https://developer.apple.com/design/human-interface-guidelines/">Human Interface Guidelines</a></h2>

<p class="feature-text">
	Guidance and best practices to help designers and developers create great experience for any Apple platform.
</p>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% for feature in site.data.designs %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<br>
<h2 class="feature-title">Featured <a href="/cv/#interactive-articles">Interactive Articles</a></h2>

<p class="feature-text">
	Enhanced reading experiences that demonstrate what's possible when dynamic media are effectively combined.

</p>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedArticles = site.data.articles | where: "featured", true %}
	{% assign ia = site.categories.papers | where:"permalink", "papers/interactive-articles" %}

	{% assign feature = sortedArticles[1] %}
	{% include feature.html feature=feature %}

	{% assign feature = sortedArticles[0] %}
	{% include feature.html feature=feature %}

	{% assign feature = ia[0] %}
	{% include feature.html feature=feature %}
</div>

<br>
<h2 class="feature-title"><a href="https://parametric.press/about">Parametric Press</a></h2>

<p class="feature-text">
	A born-digital, experimental magazine dedicated to showcasing the expository power of the web.
</p>

<div class="cover-wrapper cover-wrapper-2-col l-middle">
	{% assign parametric = site.data.articles | where: "parametric-issue", true %}
	{% for feature in parametric %}
		{% include feature.html feature=feature %}
	{% endfor %}
</div>
{% endcomment %}



[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[alex]: http://va.gatech.edu/endert/ "Alex Endert"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[nstrf]: https://www.nasa.gov/strg/nstrf "NASA Space Technology Research Fellowship"