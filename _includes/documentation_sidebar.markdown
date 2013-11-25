{% assign t = site.tags.translations[0] %}
        {% assign url_lang = '' %}        
        {% if page.lang == 'en' %}{% assign url_lang = 'en/'%}{% endif %}
<div class="well">
	<h3>{{t.[page.lang].menu.documentation}}</h3>
	<ul>
		<li><a href="/{{url_lang}}dokumentation/komigang">{{t.[page.lang].menu.guide}}</a></li>
		<li><a href="/{{url_lang}}dokumentation/vagval">{{t.[page.lang].menu.choices}}</a></li>
		<li><a href="/{{url_lang}}dokumentation/licens">{{t.[page.lang].menu.license}}</a></li>
		<li><a href="/{{url_lang}}dokumentation/begransningar">{{t.[page.lang].menu.limitations}}</a></li>
		<li><a href="/{{url_lang}}dokumentation/villkor">{{t.[page.lang].menu.conditions}}</a></li>
		<li><a href="/{{url_lang}}dokumentation/rattsligaval">{{t.[page.lang].menu.legal_options}}</a></li>
		<li><a href="/{{url_lang}}dokumentation/affarsval">{{t.[page.lang].menu.business_options}}</a></li>
		<li><a href="/{{url_lang}}dokumentation/bilagor">{{t.[page.lang].menu.attachments}}</a></li>
	</ul>
</div>