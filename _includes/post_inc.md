
 <div style="margin-top:24px; margin-bottom:24px; border-bottom: 1px solid #eee;">

<a href="{{ post.url | prepend: site.baseurl }}" class="catalogue-item"> 
     {% if post.cover %}
       <img class="post_cover_img" src="{{ post.cover }}" height="200px" width="200px" border="1px" style="border: 0px solid #ddd; padding-right:12px;padding-top:12px; margin-right: 12px;">
     {% else %}
       <img class="post_cover_img" src="{{ site.cover }}" height="200px" width="200px" border="1px" style="border: 0px solid #ddd; padding-right:12px;padding-top:12px; margin-right: 12px;">
     {% endif %}
    </a>
     <div class="catalogue-item post_box"> 
       
<a href="{{ post.url | prepend: site.baseurl }}" class="catalogue-item">
       <h1 class="catalogue-title">{{ post.title }}</h1>
       <div class="catalogue-line"></div>
       <p> {{ post.content | strip_html | truncatewords: 30 }} </p>
       </a>
       <time datetime="{{ post.date }}" class="catalogue-time">{{ post.date | date: "%Y-%m-%d" }}</time>
		<p style="float:right; padding:0; margin:0; ">
		{% for category in post.categories %}
			{% if category == "haz" %}
				<a href="/haz" style="padding:0; margin:0;">Házfelújítás</a> &nbsp;
			{% endif %}
			
			{% if category == "dekor" %}
				<a href="/dekor" style="padding:0; margin:0;">Dekoráció</a>  &nbsp;
			{% endif %}
			{% if category == "dekor" %}
				<a href="/kert" style="padding:0; margin:0;">Keti ötletek</a>  &nbsp;
			{% endif %}
		{% endfor %}
		</p>
     </div>
 </div>

