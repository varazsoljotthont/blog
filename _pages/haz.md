---
layout: default
permalink: /haz/
title: Házfelújítás
---


<p align="right" style="color:#880015"><strong>Téglából ház, lélekből otthon!</strong></p>


<h2 style="text-align:center; padding-top: 48px; padding-bottom:48px; line-height:48px;">Egy régi ház felújításának története leírásokkal, képekkel, tapasztalatokkal... <br>
Ötletek, inspriációk a házunk tájáról
 </h2>


<div class="catalogue">
{% for post in site.categories.haz %}
  {% capture my_include %}{% include post_inc.md %}{% endcapture %}
	{{ my_include | markdownify }}
{% endfor %}
</div>

