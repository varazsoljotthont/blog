---
layout: default
permalink: /kert/
title: Kerti ötletek
---


<p align="right" style="color:#880015"><strong>Téglából ház, lélekből otthon!</strong></p>


<h2 style="text-align:center; padding-top: 48px; padding-bottom:48px; line-height:48px;">Kertünk, udvarunk átalakulásának, építésének  története ilyen volt -ilyen lett képekkel, fa és bontott tégla felhasználásával készült pihenőhelyekkel, olcsó és házilag is kivitelezhető ötletekkel, praktikákkal, leírásokkal<br> 
	Számomra a kert a színek, formák, illatok tánca. <br>Öröm, boldogság, sikerélmény...</h2>

<div class="catalogue">
{% for post in site.categories.kert %}
  {% capture my_include %}{% include post_inc.md %}{% endcapture %}
	{{ my_include | markdownify }}
{% endfor %}
</div>

