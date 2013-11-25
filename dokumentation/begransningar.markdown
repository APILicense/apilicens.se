---
layout: post
lang: se
title:  "Licensens innehåll och begränsningar"
date:   2013-11-18 13:23:00
---
Följande förtydliganden och begränsningar gäller med avseende på vilka typer av API:er som ska kunna tillhandahållas under licensen, och de frågor som omfattas av licensen:

Licensen täcker:

* Webbaserade API:er, typiskt realiserade genom tekniska protokoll som REST och SOAP.
* API:er som både läser och skriver information.
* API:er tillhandahållna av företag. 
* API:er som är gratis att använda, som tillhandahålls mot betalning eller en kombination av dessa två varianter. 

Licensen täcker inte:

* Verktyg, programkod eller kodbibliotek som bygger på API:et.
* API:er som tillhandahålls av myndigheter och andra offentliga enheter. De står under legala krav på offentlighet och sekretess m.m. som inte har beaktats i projektet.
* API:er som stöder beställningar och/eller köp av varor via själva API:et. Konsumenters beställningar och köp av varor i en digital miljö aktualiserar bestämmelser om informationsskyldighet, ångerrätt m.m. som det inte finns utrymme för inom projektets ramar.
* Legala informationskrav som behöver uppfyllas i samband med att ett företag tillhandahåller ett API, men som inte behöver omnämnas i själva licenstexten, utan t.ex. på den webbplats som API:et tillhandahålls på. Som exempel på sådana krav kan nämnas informationskraven i §§ 10-12 lag (2002:562) om elektronisk handel och andra informationssamhällets tjänster och informationskraven i distans- och hemförsäljningslag (2005:59).

{% sidebar %}
{% include documentation_sidebar.markdown %}
{% endsidebar %}

<script>
$( document ).ready(function() {
	$('.navbar li.active').removeClass('active');		    
	$('.navbar li#menu_limitations').addClass('active');		
	$('.navbar li#menu_documentation').addClass('active');		    
});
</script>