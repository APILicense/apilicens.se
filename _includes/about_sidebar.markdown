{% assign t = site.tags.translations[0] %}
{% assign url_lang = '' %}        
{% if page.lang == 'en' %}{% assign url_lang = 'en/'%}{% endif %}
<div class="well">
	<h3>{{t.[page.lang].menu.about}}</h3>
	<ul>
		<li><a href="/{{url_lang}}om/projektet">{{t.[page.lang].menu.project}}</a></li>
		<li><a href="/{{url_lang}}om/press">{{t.[page.lang].menu.press}}</a></li>
		<li><a href="/{{url_lang}}om/logotyper">{{t.[page.lang].menu.logotypes}}</a></li>
		<li><a href="/{{url_lang}}om/kontakta">{{t.[page.lang].menu.contact}}</a></li>
	</ul>
</div>