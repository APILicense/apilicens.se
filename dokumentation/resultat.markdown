---
layout: post
lang: se
title:  "Licensvillkor för API - resultat från wizard"
date:   2013-12-03 12:58:00
---
<script>
$( document ).ready(function() {

	var hideShowOptions = function(n){
		if ($.url().param(n) == "n") {
			$('.choice'+n+'y').parent('li').remove(); //Remove list item in the "left to do" list
			$('.choice'+n+'y').remove();
			$('.choice'+n).remove();
			$('#response'+n).html('Nej');
		}
		else if ($.url().param(n) == "y") {
			$('.choice'+n+'n').parent('li').remove();
		 	$('.choice'+n+'n').remove();
			$('.choice'+n).remove();
		}	
		else {
			$('#response'+n).html('Inget val gjort');	
		}
	}

	var choices = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12", "13"];
	$.each(choices, function(index, value){
		hideShowOptions(value);
	});
	
	//To remove section 3 completely if it contains no content
	if (($.url().param("4") == "n") && ($.url().param("5") == "n")) {
		$('#3').remove();
	}	

});
</script>

Licensen nedan är baserad på följande [vägval](/dokumentation/wizard):

* Kommer API:et att lämna ut immaterialrättsligt skyddat material? - **<span id="response1">Ja</span>**
* Ska API-användaren hänvisa till datakällan?  - **<span id="response2">Ja</span>**
* Vill du ha rätt att hänvisa till API-användarens varumärke/firma? - **<span id="response3">Ja</span>**
* Kommer API-användaren att behöva registrera sina personuppgifter för att få ta del av API:et? - **<span id="response4">Ja</span>**
* Kommer API:et att lämna ut personuppgifter? - **<span id="response5">Ja</span>**
* Finns det tekniska begränsningar i hur användaren får använda API-innehållet? - **<span id="response6">Ja</span>**
* Kommer du att vilja ta betalt för användandet av API:et? - **<span id="response7">Ja</span>**
* Finns begränsningar med avseende på kommersiell användning av information från API:et? - **<span id="response8">Ja</span>**
* Vill du begränsa användningen av API:et för syften som riskerar att skada din verksamhet? - **<span id="response9">Ja</span>**
* Ska API:ets användare ha möjlighet att rapportera fel/brister i den information som hämtas? - **<span id="response10">Ja</span>**
* Lämnas några garantier för informationens kvalitet och korrekthet? - **<span id="response11">Ja</span>**
* Kommer API-användaren att kunna generera information till API:et? - **<span id="response12">Ja</span>**
* Ska det finnas begränsningar i API-användarens rätt att säga upp licensen? - **<span id="response13">Ja</span>**

Kvar att göra nu är:

* **<a href="#0">Bakgrund</a>** - Infoga tillhandahållarens namn samt webbplats, ersätt dessutom *Namn* i resten av licensen med namnet på tillhandahållaren
* <span class="choice1y">**<a href="#2.2">2.2</a>** - Infoga information om immateriella rättigheter samt licensvillkor för innehåll</span>
* <span class="choice2y">**<a href="#2.3">2.3</a>** - Infoga beskrivning av metod för hänvisning</span>
* <span class="choice4y">**<a href="#3.1">3.1</a>** - Ange länk till policy för personuppgiftsbehandling</span>
* <span class="choice6y">**<a href="#4.1">4.1</a>** - Ange länk till teknisk dokumentation samt uppdatera listan på ev. tekniska begränsningar</span>
* <span class="choice7y">**<a href="#5.2">5.2</a>** - Ange länk till prislistan</span>
* <span class="choice9y">**<a href="#5.4">5.4</a>** - Infoga beskrivning vad som riskerar att skada tillhandahållarens intressen</span>
* <span class="choice10y">**<a href="#6.1">6.1</a>** - Infoga epost-adress för felrapportering</span>
* <span class="choice11y">**<a href="#6.2">6.2</a>** - Infoga beskrivning av garanti</span>
* <span class="choice11n">**<a href="#6.2">6.2</a>** - Ange länk till teknisk dokumentation och länk till policy för ändringshantering</span>
* **<a href="#7.1">7.1</a>** - Ange länk till policy för ändringshantering
* **<a href="#8.2">8.2</a>** - Ange länk till policy för ändringshantering
* <span class="choice13y">**<a href="#8.3">8.3</a>** - Ange uppsägningstid, hur man säger upp avtalet etc</span>
* <span class="choice13n">**<a href="#8.3">8.3</a>** - Infoga beskrivning av hur man avbryter tillgång till API:et</span>

##<a id="0">Bakgrund</a>
[*Infoga tillhandahållares namn*]&nbsp;(”[**Namn**]”) tillhandahåller på webbplatsen [Infoga webbplats] ett API (”**API:et**”) som ger dig tillgång till information, kod och annat material (”**API-innehåll**”). 

Dessa licensvillkor (”**Avtalet**”) beskriver under vilka förutsättningar API:et tillhandahålls, hur vi förväntar oss att du använder API:et och vad du har rätt respektive skyldighet att göra då du använder API-innehållet i dina egna produkter eller tjänster. 

Genom att godkänna detta Avtal intygar du att du har läst, förstått och godkänner de villkor som anges häri, och de dokument till vilka Avtalet hänvisar. 

##<a id="1">1. Licens</a>
[*Namn*] beviljar dig härmed en icke-exklusiv, icke överlåtbar, icke upplåtbar och återkallbar licens att använda API:et i enlighet med detta Avtal. Denna licens, och de produkter och tjänster som du utvecklar under licensen, inte innebära någon begränsning i [*Namn*]s eller våra datakällors rätt att fritt utnyttja, utveckla, ändra och att sluta att tillhandahålla API:et, API-innehållet och tillhörande produkter och tjänster.

Som framgår nedan kommer vi dock att hålla dig uppdaterad om förändringar i API:et och våra möjligheter att tillhandahålla API:et. 

##<a id="2">2. Immateriella rättigheter</a>
**<a id="2.1">2.1</a>** [*Namn*] och/eller de tredje parter med vilka vi samarbetar innehar äganderätten och de immateriella rättigheterna till API:et. Såvida du inte har fått vårt särskilda, skriftliga godkännande har du därför inte rätt att hävda äganderätt till, publicera, kopiera, överlåta, licensiera eller annars på annat immaterialrättsligt relevant sätt förfoga över API:ets källkod eller anropsstruktur.

<span class="choice1y">**<a id="2.2">2.2</a>** API-innehållet innefattar material som skyddas av immateriella rättigheter, såsom upphovsrätt och varumärkesskydd, och du har inte rätt att hävda äganderätt till, publicera, kopiera, överlåta, licensiera eller ändra sådant material annat än i enlighet med de licensvillkor som gäller för respektive verk.][*Infoga information om hur API-användaren kan veta vilket API-innehåll som är skyddat av immateriella rättigheter och vilka licensvillkor som gäller för sådant material, t.ex. genom en hänvisning till tillämplig Creative Commons-licens.*</span>

**<a id="2.3">2.3</a>** <span class="choice2y">I samband med att API-innehållet används i av dig utvecklade produkter eller tjänster är du skyldig att i produkten respektive tjänsten ange att den innehåller data från API:et, och att hänvisa till API:et genom att [*infoga beskrivning av metod för hänvisning*]. Din rätt att använda [*Namn*]s firma och varumärke är begränsad till källhänvisningar som sker på detta vis och i detta syfte, och du har således inte rätt att använda vår firma eller våra varumärken annat än vad som uttryckligen anges i denna punkt. </span><span class="choice2n">I samband med att API-innehållet används i av dig utvecklade produkter eller tjänster har du inte rätt att hänvisa till API:et eller till [*Namn*]s firma eller varumärken.</span>

<span class="choice3y">**<a id="2.4">2.4</a>** [**Alt**: Genom att ansluta dig till API:et ger du [*Namn*] en icke exklusiv, icke överlåtbar och icke upplåtbar licens att hänvisa till din firma och de eventuella produkter och tjänster som du använder API-innehållet i (inklusive eventuella varumärken som du innehar för sådana produkter eller tjänster), i syfte att informera om att du använder dig av API:et. [*Namn*]s rätt att använda din firma och varumärken är begränsad till källhänvisningar som sker i detta syfte.]</span>

##<a id="3">3. Personuppgiftsbehandling</a>
<span class="choice4y">**<a id="3.1">3.1</a>** I samband med att du väljer att ansluta dig till API:et kan du behöva registrera vissa personuppgifter hänförliga till dig. Genom att registrera dina personuppgifter samtycker du till att [*Namn*] behandlar dina personuppgifter i syfte att administrera, övervaka och möjliggöra din användning av API:et, och att [*Namn*] i egenskap av personuppgiftsansvarig i enlighet med personuppgiftslag (1998:204), behandlar dina personuppgifter i enlighet med vår Policy för personuppgiftsbehandling [*Ange länk till denna policy*]. </span>

<span class="choice5y">**<a id="3.2">3.2</a>** API-innehållet innefattar personuppgifter, och du är medveten om och accepterar att du genom att inhämta, använda, sammanställa, sprida eller i övrigt behandla sådana personuppgifter är personuppgiftsansvarig för denna behandling i enlighet med personuppgiftslag (1998:204).</span>

##<a id="4">4. Tekniska krav och begränsningar</a>
<span class="choice6y">**<a id="4.1">4.1</a>** För att säkerställa och upprätthålla API:ets och API-innehållets tillgänglighet och kvalitet är du skyldig att följa våra instruktioner avseende [cachening, lagring, kopiering och uppdatering] av API-innehållet som framgår av vår Tekniska Dokumentation [*Ange länk till dokumentationen*].</span>

**<a id="4.2">4.2</a>** Du får bara ansluta till API:et på det sätt som följer av våra instruktioner, och har inte rätt att på teknisk väg bereda dig obehörig tillgång till, störa eller avaktivera API:et. Det här innebär, men är inte begränsat till, att du åtar dig att inte sprida virus, maskar, trojaner eller annan skadlig kod i API:et eller på den webbplats där API:et tillhandahålls. 

##<a id="5">5. Övriga krav på din användning </a>
**<a id="5.1">5.1</a>** Du behöver ha fyllt 18 år för att ha rätt att ingå detta Avtal, och för att få tillgång till API:et.

<span class="choice7y">**<a id="5.2">5.2</a>** Din tillgång till API:et och API-innehållet är villkorat av att du betalar för din användning i enlighet med de priser och betalningsvillkor som framgår av vår Prislista [*Ange länk till prislistan*].</span>

<span class="choice8y">**<a id="5.3">5.3</a>** [**Alt. 1**: Du har inte rätt att använda API-innehållet i någon typ av kommersiellt syfte. Det här innebär att du inte har rätt att använda API-innehållet i en produkt eller tjänst som på något vis genererar inkomster, inklusive men inte begränsat till genom reklamfinansiering eller krav på betalning för medlemskap eller prenumeration.]</span>

<span class="choice8y">[**Alt**.2: Din rätt att använda API-innehållet i kommersiellt syfte är begränsad genom att du inte har rätt att ta betalt av användaren för de produkter och tjänster där du använder API-innehållet. Du har emellertid rätt att använda API-innehållet för produkter eller tjänster som är reklamfinansierade.]</span>

<span class="choice9y">**<a id="5.4">5.4</a>** Du har inte rätt att använda API:et eller API-innehållet för produkter eller tjänster som riskerar att skada [*Namn*]s verksamhet eller stå i strid med våra intressen. Det här innebär att API:et och API-innehållet inte får användas för produkter eller tjänster som [*infoga beskrivning av produkter/tjänster/sammanhang som riskerar att skada tillhandahållarens intressen.*]</span>

**<a id="5.5">5.5</a>** Du har inte rätt att använda API:et eller API-innehållet för produkter eller tjänster som bryter mot, eller som uppmanar till brott mot, tillämpliga lagar och förordningar.

**<a id="5.6">5.6</a>** Om du har några frågor om innebörden av de begränsningar som framgår av denna punkt ”Övriga krav på din användning” eller vill använda API:et eller API-innehållet på något annat sätt än vad som framgår häri kan du kontakta oss på [infoga e-postadress]. Du har dock inte rätt att påbörja sådan annan användning förrän du har fått vårt skriftliga godkännande. 

##<a id="6">6. Ansvar</a>
<span class="choice10y">**<a id="6.1">6.1</a>** Vi strävar efter att löpande förbättra API:et och ser gärna att du informerar oss om eventuella fel eller brister i användarupplevelsen genom att skicka ett meddelande till [*infoga epost-adress*]. Som närmare anges i denna punkt ”Ansvar” har vi dock begränsade möjligheter att åtgärda fel eller problem.</span>

**<a id="6.2">6.2</a>** <span class="choice11y">Vi lämnar följande, begränsade garanti för API:et och API-innehållet: [*infoga beskrivning av garanti.*]. I övrigt accepterar du att [*Namn*] inte lämnar några utfästelser eller garantier avseende API:ets eller API-innehållets kvalitet, säkerhet, tillförlitlighet, tillgänglighet eller prestanda.</span><span class="choice11n">Du är medveten om och accepterar att [*Namn*] inte lämnar några utfästelser eller garantier avseende API:ets eller API-innehållets kvalitet, säkerhet, tillförlitlighet, tillgänglighet eller prestanda. Oavsett vad som framgår av vår Tekniska Dokumentation [*Ange länk till dokumentationen*], Policy för Ändringshanteringar [*Ange länk till denna policy*] eller eventuella beskrivningar av API:ets funktion i samband med att API:et tillhandahålls kan du således inte förvänta dig att API:et kommer att vara fritt från fel, fritt från säkerhetsproblem, uppdaterat eller en lämplig datakälla för de produkter eller tjänster du avser att använda det i.</span>

**<a id="6.3">6.3</a>** Du är medveten om och accepterar att du använder API:et på egen risk, och att [*Namn*] inte ansvarar för eventuella indirekta skador som uppstår för dig på grund av att du har använt, respektive inte har kunnat använda, API:et eller API-innehållet. Med indirekta skador avses i detta Avtal exempelvis utebliven vinst, utebliven användning av dina produkter eller tjänster, ersättning för användning av en ersättande tjänst, förlust av data, kostnader för felsökning, goodwillskador och skador på grund av virus och andra säkerhetsrelaterade problem. Du accepterar också att [*Namn*]s sammanlagda ersättningsskyldighet till dig på grund av att du har använt, respektive inte har kunnat använda, API:et eller API-innehållet är begränsad till [*infoga summa*].

<span class="choice12y">**<a id="6.4">6.4</a>** Om du som användare genererar data och information till API:et accepterar du att du själv ansvarar för att du har rätt att publicera och sprida sådan information, innefattande men inte begränsat till att du (i) inte agerar i strid med annans immateriella rättigheter; (ii) har laglig grund att sprida eventuella personuppgifter; (iii) inte sprider uppgifter som bryter mot, eller som uppmanar till brott mot, tillämpliga lagar och förordningar.</span>

**<a id="6.5">6.5</a>** Du åtar dig att hålla [*Namn*], våra samarbetspartners och anställda skadeslösa för eventuella krav från tredje parter med anledning av din användning av API:et eller API-innehållet i strid med detta Avtal. 

##<a id="7">7. Förändringar</a>
**<a id="7.1">7.1</a>** Vi förbehåller oss rätten att uppdatera och ändra API:et, API:ets innehåll och detta Avtal i enlighet med vår Förändringspolicy. Av policyn för ändringshantering [*Ange länk till denna policy*] framgår vilka förändringar som kan komma att ske, hur förändringar kommuniceras till dig, och med vilken framförhållning.

**<a id="7.2">7.2</a>** Ändringar i detta Avtal dokumenteras genom att vi ger ut en ny version av villkoren. Varje ny version av villkoren kommer att förses med ett nytt versionsnummer i dokumentets slut. 

**<a id="7.3">7.3</a>** Genom att fortsätta att använda API:et efter att en förändring har genomförts intygar du att du godkänner förändringen. Om du inte vill acceptera en förändring har du inte längre rätt att använda API:et och måste avbryta din anslutning till API:et i enlighet med punkten ”Avtalstid och Uppsägning” nedan. 

##<a id="8">8. Avtalstid och uppsägning</a>
**<a id="8.1">8.1</a>** Detta Avtal, och din licens till API:et, träder i kraft då du godkänner Avtalet och är giltigt så länge [*Namn*] tillhandahåller API:et, såvida det inte sägs upp i förtid i enlighet med denna punkt ”Avtalstid och Uppsägning”.

**<a id="8.2">8.2</a>** [*Namn*] förbehåller sig rätten att säga upp detta Avtal till omedelbart upphörande och att stänga av din anslutning till API:et om du använder API:et eller API-innehållet i strid med vad som anges häri. Vi förbehåller oss också rätten att, efter egen skälig bedömning och efter föregående meddelande till dig i enlighet med vår Förändringspolicy [*Ange länk till denna policy*], permanent eller tillfälligt sluta att tillhandahålla hela eller delar av API:et eller API-innehållet.

**<a id="8.3">8.3</a>** <span class="choice13y">Du har rätt att säga upp detta Avtal förutsatt att du [*ange uppsägningstid, metod för uppsägning och ev. kostnad för uppsägning i förtid.*]</span><span class="choice13n">Du har rätt att när som helst, utan särskilt skäl och utan kostnad säga upp detta Avtal. Sådan uppsägning sker genom att du avbryter din anslutning till API:et, genom att [*infoga beskrivning av hur man avbryter tillgång till API:et.*].</span>

**<a id="8.4">8.4</a>** Om din rätt att använda API.et upphör är du skyldig att med omedelbar verkan avsluta och radera din anslutning till API:et<span class="choice2y"> och eventuella hänvisningar till vår firma och våra varumärken som används i dina produkter eller tjänster</span>.

##<a id="9">9. Övrigt</a>
**<a id="9.1">9.1</a>** Detta Avtal utgör den fullständiga regleringen av alla frågor rörande din rätt att använda API:et och API-innehållet. Ändringar i eller tillägg till detta Avtal utöver nya versioner enligt punkten ”Förändringar” ovan ska, för att äga giltighet, ske genom skriftlig bekräftelse från [*Namn*].

**<a id="9.2">9.2</a>** Du har inte rätt att överlåta dina rättigheter och skyldigheter enligt detta Avtal till en tredje part. [*Namn*] förbehåller sig rätten att, efter särskilt meddelande till dig, överlåta Avtalet till företag inom vår koncern och till en tredje part som förvärvar hela eller delar av vår verksamhet. 

**<a id="9.3">9.3</a>** I den mån som någon av dina skyldigheter eller någon begränsning av dina rättigheter enligt detta Avtal, på grund av dina rättigheter som konsument, inte är tillåten enligt lag ska de inte vara gällande gentemot dig. Inget i Avtalet avser således att utesluta eller begränsa rättigheter som du som konsument har enligt lag.

**<a id="9.4">9.4</a>** Detta Avtal ska styras av och tolkas i enlighet med svensk rätt. Eventuella tvister som uppstår i anledning av detta Avtal ska avgöras av svensk domstol.

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Licensvillkor för API</h3>
<ol>	
	<li><a href="#1">Licens</a></li>
	<li><a href="#2">Immateriella rättigheter</a></li>
	<li><a href="#3">Personuppgiftsbehandling</a></li>
	<li><a href="#4">Tekniska krav och begränsningar</a></li>
	<li><a href="#5">Övriga krav på din användning</a></li>
	<li><a href="#6">Ansvar</a></li>
	<li><a href="#7">Förändring</a></li>
	<li><a href="#8">Avtalstid och uppsägning</a></li>
	<li><a href="#9">Övrigt</a></li>
<ol>
</div>
{% endsidebar %}

<script>
$( document ).ready(function() {
	$('.navbar li.active').removeClass('active');		    
	$('.navbar li#menu_license').addClass('active');		
	$('.navbar li#menu_documentation').addClass('active');		    
});
</script>