---
layout: post
lang: se
title:  "Kom igång med licensen"
date:   2013-11-21 10:21:00
---
Om du behöver en användarlicens för ett API så följ dessa steg...

##1. Passar licensen?
För att veta om licensen passar ett API så läs igenom vilka [begränsningar](/dokumentation/begransningar) och [villkor](/dokumentation/villkor) som gäller. Sammanfattningsvis så är licensen anpassad för företag som tillhandahåller webbaserade APIer och att licensen måste godkännas av alla API-användare. 

##2. Skräddarsy licensen
Licensen är gjord för att vara flexibel nog att stämma in på väldigt många användarfall och för att veta vilka paragrafer i licensen som ska användas i ett givet fall så gå igenom [alla rättsliga och affärsmässiga vägval](/dokumentation/vagval). 

Beroende på vilka vägval som görs så måste också lite mer information infogas i själva [licenstexten](/dokumentation/licens/), denna information är [*angiven i kursiv stil*] i licensen. Beroende på vilka val som görs så krävs också vissa [bilagor](/dokumentation/bilagor/) till licensen med ytterligare information.

När väl alla vägval är gjorda och all extrainformation infogad så är licensen redo att användas, såvida den inte behöver skräddarsys ytterligare efter just ditt API. Som framgår av [Villkor för licensen](/dokumentation/villkor/) rekommenderar vi den API-tillhandahållare som vill vara helt säker på att man har en licenstext som fullt återspeglar dina individuella förutsättningar att låta en jurist se över ditt förslag till licenstext.

Missa inte heller att hela licenstexten finns både på [svenska](/dokumentation/licens/) och på [engelska](/en/dokumentation/licens/), så det går bra att använda licensen även mot icke-svensktalande användare.

##3. Använd licensen
Ta all den skräddarsydda licenstexten från föregående steg och lägg in den i APIets dokumentation samt kräv att alla användare av APIet godkänner licensen. Det rekommenderas att licensen tydligt märks med versionsnummer och [helst görs tillgänglig](/dokumentation/rattsligaval/#aterskapa) via ett publikt versionhanteringssystem (tex [GitHub](https://github.com)). Glöm inte att alltid [hänvisa till originallicensen](/dokumentation/villkor/#hanvisning).

##4. Låt oss veta att du använder licensen
Skicka ett mail till [info@apilicens.se](mailto:info@apilicens.se) om att licensen används så listar vi mer än gärna ert projekt på denna webbsajt. 

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Kom igång med licensen</h3>
<ol>	
	<li><a href="#1">Passar licensen?</a></li>
	<li><a href="#2">Skräddarsy licensen</a></li>
	<li><a href="#3">Använd licensen</a></li>
	<li><a href="#4">Låt oss veta att du använder licensen</a></li>
<ol>
</div>
{% endsidebar %}

<script>
$( document ).ready(function() {
	$('.navbar li.active').removeClass('active');		    
	$('.navbar li#menu_guide').addClass('active');		
	$('.navbar li#menu_documentation').addClass('active');		    
});
</script>