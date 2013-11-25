---
layout: post
lang: se
title:  "Affärsmässiga vägval"
date:   2013-11-18 14:04:00
---
Detta är de affärsmässiga vägval som påverkar vilka delar av [licenstexten](/dokumentation/licens) som kommer att användas. De affärsmässiga valen är helt beroende av de strategiska val företag gör, ex. vad gäller prissättning och vidareanvändning av API:ets innehåll. Eftersom licensen innehåller de vanligaste vägvalen ett företag står inför när det ska tillhandahålla ett API är licensen anpassningsbar för många olika användningsfall

En kort version av alla val finns på [snabba vägval](/dokumentation/vagval/).

##<a id="tekniska">Tekniska krav och begränsningar</a>
Ur ett affärsmässigt perspektiv kan det vara viktigt hur API-användarna ska få cache:a, lagra och kopiera den information som hämtas via API:et.

En del information är mycket tidskritisk (ex. finansiell eller trafikrelaterad data) vilket gör att lagring kan riskera att skapa en dålig slutanvändarupplevelse. Annan information uppdateras sällan, vilket minskar risken med lokalt lagrad data. Lokal lagring av API:ets användare kan också minska belastningen på de system som API:et används på. 

Vissa företag behöver kunna förhindra att stora delar av deras data kopieras, eftersom hela företagets existens annars kan riskeras. För API:ets användare kan ett förbud mot lagring emellertid ses som hindrande, t.ex. om utvecklaren redan har en serverinfrastruktur som man vill använda eller om informationen behöver processas före visning för slutanvändare. För andra utvecklare som utvecklar tjänster som till stor del liknar API:ets utformning kan istället en direkt användning utan att en egen serverinfrastuktur behöver sättas upp ses som positivt. 

Att API-ägaren hindrar API-användarna från att lagra data kan också hindra utvecklingen av vissa typer av tjänster (tjänster som man från början kanske inte ens föreställt sig skulle utvecklas), t.ex. tjänster där statistik sammanställs och presenteras baserat på olika typer av realtidsdata.

Mot bakgrund av den här typen av avväganden bör API-tillhandahållaren bestämma huruvida man vill sätta upp några begränsningar i användarens rätt att cache:a, lagra och kopiera information från API:et, liksom om användaren i sådant fall har ett ansvar att hålla lagrad data uppdaterad.

Exakt vilka tekniska begränsningar och möjligheter som ska erbjudas användaren är upp till varje API-tillhandahållare, men projektet rekommenderar att en tillhandahållare lämnar den information som framgår av mallen för Teknisk Dokumentation. 

###Vägval i licensen
Finns det tekniska begränsningar i hur användaren får använda API-innehållet, t.ex. gällande cache:ar, lagring, kopiering och uppdatering av API-innehållet?	

* Ja: Behåll [punkt 4.1 i licenstexten](/dokumentation/licens#4.1) och stryk ev. hänvisning till begränsning som inte är aktuell.  
* Nej: Stryk [punkt 4.1 i licenstexten](/dokumentation/licens#4.1).

##<a id="betalning">Betalning för tillgång till API:et</a>
En viktig fråga för API-tillhandahållare är hur API:et ska betala sig. I vissa fall handlar det endast om ett ökat antal tjänster som gör att fler kunder eller andra intressenter kan nås på plattformar och sammanhang som stämmer med deras preferenser. I andra fall kan företaget inneha information som är svår eller omöjlig att få tag på annat sätt, och som företaget vill ta betalt för. I ytterligare andra fall tillämpas en hybridmodell, där det finns en gratisnivå och en eller flera betalnivåer (där utvecklaren får tillgång till ytterligare information eller fler anrop per given tidsenhet).

I det fall innehållet i API:et helt eller delvis är avgiftsbelagt rekommenderar projektet att licensen hänvisar till en separat prislista. 
Vägval i licensen

Kommer du att vilja ta betalt för användandet av API:et?	

* Ja: Behåll [punkt 5.2 i licenstexten](/dokumentation/licens#5.2).
* Nej: Stryk [punkt 5.2 i licenstexten](/dokumentation/licens#5.2). 

##<a id="kommersiell">Kommersiell användning av information från API:et</a>
Att möjliggöra kommersiell användning av ett API är ofta något som gör det mer attraktivt för API-användarna att utveckla tjänster på API:et, men i vissa fall vill en API-tillhandahållare inte att externa utvecklare bygger tjänster som tjänar pengar på dess egen information.

Om en API-tillhandahållare vill begränsa möjligheten att använda information från API:et i kommersiella syften är det viktigt att sätta upp tydliga gränser för vad som ska anses vara kommersiell användning. Får till exempel API:ets användare utveckla en tjänst som innehåller reklam?

###Vägval i licensen
Finns begränsningar med avseende på kommersiell användning av information från API:et? 	

* Ja: Behåll något av alternativen i p[punkt 5.3 i licenstexten](/dokumentation/licens#5.3) eller ange en egen begränsning
* Nej: Stryk [punkt 5.3 i licenstexten](/dokumentation/licens#5.3).

##<a id="hanvisning">Hänvisning till källa</a>
Att ange varifrån information från API:et har hämtats, t.ex. genom att använda API-ägarens logotyp, kan beroende på tjänst generera både positiva och negativa effekter för API-ägaren. Många API-ägare väljer att tillhandahålla speciella varumärken eller guidelines för denna situation, t.ex. ”Powered by XXX”. Att ställa krav på API-användaren att denna information ska framgå kan dock vara orimligt, t.ex. om tjänsten använder en stor mängd datakällor som ställer samma krav, så att hela tjänsten dränks med källinformation. 

Det är viktigt att utforma en API- licensen så att rimliga krav ställs i detta avseende. I licensen bör det tydligt framgå vilka krav som ställs på hänvisning till källan. Typiskt kan detta innebära att

* Ingen hänvisning får ske (d.v.s. datakällan ska vara helt anonym).
* Namn/logotyp/länk till datakällan ska visas för slutanvändaren så att det tydligt framgår vilka datakällor som används. 
* Varje del av den data som kommer från API:et måste märkas på ett sådant sätt att slutanvändaren förstår exakt var just den aktuella datamängden kommer ifrån.

Användarens skyldighet att hänvisa till datakällan bör upphöra när/om användarens licens att använda API:et upphör (jfr. punkt 8.4 i licenstexten). 

Vissa tillhandahållare av API:er vill också själva ha rätt att ange användarens varumärke eller firma för att annonsera vem som använder sig av API:et.

###Vägval i licensen
Ska API-användaren hänvisa till datakällan?	

* Ja: Behåll Alt.1 i [punkt 2.3 i licenstexten](/dokumentation/licens#2.3) och infoga efterfrågad information. Stryk Alt. 2. Behåll också den markerade texten i [punkt 8.4 i licenstexten](/dokumentation/licens#8.4).
* Nej:. Behåll Alt.2 i [punkt 2.3 i licenstexten](/dokumentation/licens#2.3). Stryk Alt.1. Stryk också den markerade texten i [punkt 8.4 i licenstexten](/dokumentation/licens#8.4).

Vill du som API-tillhandahållare ha rätt att hänvisa till API-användarens varumärke/firma?	

* Ja: Behåll [punkt 2.4 i licenstexten](/dokumentation/licens#2.4).
* Nej: Stryk [punkt 2.4 i licenstexten](/dokumentation/licens#2.4).

##<a id="kvalitet">Kvalitet och korrekthet</a>
###Anmälan om fel eller brister
För den API-tillhandahållare som vill hålla hög kvalitet och korrekthet i data som tillhandahålls via API:et rekommenderar projektet att en särskild kontaktväg för anmälan om fel i data tillhandahålls, t.ex. en e-postadress till vilken API:ets användare kan meddela eventuella upptäckta fel eller brister i hämtad data. Det förutsätter dock självklart att tillhandahållaren faktiskt har resurser för att läsa och följa upp de anmälningar som görs. 

####Vägval i licensen
Ska API:ets användare ha möjlighet att rapportera fel eller brister i den information som hämtas?	

* Ja: Behåll [punkt 6.1 i licenstexten](/dokumentation/licens#6.1) och infoga efterfrågad information.
* Nej: Stryk [punkt 6.1 i licenstexten](/dokumentation/licens#6.1).

###<a id="garantier">Garantier</a>
En vanligt återkommande fråga för API-tillhandahållare är vem som ansvarar för API-informationens kvalitet och korrekthet. Ofta handlar det om vem som kan hållas ansvarig om t.ex. ett API returnerar felaktig information som sedan drabbar slutanvändaren, d.v.s. den som utnyttjar API-användarens tjänster. 

Ansvaret kan dels gälla den information som API-tillhandahållaren har genererat, och dels information som genererats av API:ets användare, om API:et tillåter att information skrivs tillbaka till API-tillhandahållaren. 

Huruvida API-tillhandahållaren ska ta på sig något ansvar för den information som man själv har genererat är en rent affärsmässig fråga, där en utslagsgivande faktorn är i många fall är om API:et tillhandahålls mot betalning eller inte, eftersom en användare som betalar för tillgång till ett API kan anses ha skälig grund att ha högre förväntningar på informationens kvalitet än någon som får informationen gratis. 

Projektet rekommenderar dock att man som tillhandahållare är försiktig med att lova för mycket, och att man – om man överhuvudtaget ska lämna några garantier för API-innehållets kvalitet, tillförlitlighet etc. – bara utlovar SLA-nivåer, lämnar utfästelser om korrekthet etc. som man är säker på att man kan uppfylla. 

Som framgår av [punkt 6.3 i licenstexten](/dokumentation/licens#6.3) rekommenderar projektet att en API-tillhandahållare avsäger sig ansvar från indirekta skador såsom utebliven vinst m.m., eftersom sådana skador är mycket svåra att förutsäga och därmed att ”ta höjd för”. API-tillhandahållaren bör också sätta en beloppsbegränsning för sitt ansvar. 

I det fall som API:ets användare kan generera information till API:et bör det framgå av licenstexten att användaren ansvarar för att han eller hon har nödvändiga rättigheter till den information som användaren gör tillgänglig (avseende t.ex. upphovsrätt och varumärken), och att användaren i övrigt ska ha rätt att sprida informationen, exempelvis genom att han eller hon har laglig grund att sprida ev. personuppgifter som överförs. 

###Vägval i licensen 
Lämnas några garantier för informationens kvalitet och korrekthet?	

* Ja: Behåll Alt.1 i [punkt 6.2 i licenstexten](/dokumentation/licens#6.2) och ange efterfrågad information. Stryk Alt.2.
* Nej: Behåll Alt.2 i [punkt 6.2 i licenstexten](/dokumentation/licens#6.2). Stryk Alt.1.

Kommer API-användaren att kunna generera information till API:et?	

* Ja: Behåll [punkt 6.4 i licenstexten](/dokumentation/licens#6.4). 
* Nej: Stryk [punkt 6.4 i licenstexten](/dokumentation/licens#6.4). 

##<a id="forandring">Hantering av förändringar i API:et</a>
I förvaltningen av öppna APIer krävs att förändringar hanteras på ett strukturerat sätt, vad gäller såväl tekniska förändringar i själva API:et som förändringar i prisförutsättningar och i licenstexten. 

Strukturen för förändringshantering bör kommuniceras till API:ets användare för att skapa realistiska förutsättningar för hur en utvecklare kommer att kunna använda API:et.

Förutsättningarna för hantering av förändringar tenderar att variera mellan olika API-tillhandahållare och kräver relativt detaljerade förklaringar, men projektet rekommenderar att en tillhandahållare lämnar åtminstone den information som framgår av mallen för en Förändringspolicy. 

###Implikation för licensen
Se [punkt 7.1 i licenstexten](/dokumentation/licens#7.1).

##<a id="skada">Skada och avstängning</a>
Det händer att en API-tillhandahållare begränsar användningen av API:et genom att ange att API:et inte får användas för att utveckla tjänster som skadar API-ägaren, t.ex. genom att tjänsten i fråga strider mot API-ägarens värderingar eller motverkar API-ägarens verksamhet. 

För att denna typ av skrivningar ska vara förståelig för API-användarna är det viktigt att det är tydligt vad som avses med API-tillhandahållarens värderingar respektive vad som ska kunna anses skada API-tillhandahållarens verksamhet. 

###Vägval i licensen
Vill du begränsa användningen av API:et för syften som riskerar att skada din verksamhet?

* Ja: Behåll [punkt 5.4 i licenstexten](/dokumentation/licens#5.4) och infoga efterfrågad information.
* Nej: Stryk [punkt 5.4 i licenstexten](/dokumentation/licens#5.4)

##<a id="uppsagning">Uppsägning</a>
I de fall som användaren har betalat för att få tillgång till API:et (t.ex. genom en prenumeration) kan API-tillhandahållaren vilja sätta upp begränsningar i användarens rätt att säga upp avtalet, genom att föreskriva att man måste lämna meddelande om uppsägning ett visst antal veckor i förväg eller genom att användaren förvisso kan säga upp sin anslutning med omedelbar verkan, men i sådant fall måste ersätta tillhandahållaren för den återstående, avtalade tiden. 

###Vägval i licensen
Ska det finnas begränsningar i API-användarens rätt att säga upp licensen?	

* Ja: Behåll Alt.1 i [punkt 8.3 i licenstexten](/dokumentation/licens#8.3) och ange efterfrågad information. Stryk Alt.2.
* Nej: Behåll Alt.2 i [punkt 8.3 i licenstexten](/dokumentation/licens#8.3) och ange efterfrågad information. Stryk Alt. 1.

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Affärsmässiga vägval</h3>
<ul>
	<li><a href="#tekniska">Tekniska krav och begränsningar</a></li>
	<li><a href="#betalning">Betalning för tillgång till APIet</a></li>
	<li><a href="#kommersiell">Kommersiell användning av information från API:et</a></li>
	<li><a href="#hanvisning">Hänvisning till källa</a></li>
	<li><a href="#kvalitet">Kvalitet och korrekthet</a></li>
	<li><a href="#forandring">Hantering av förändringar i APIet</a></li>
	<li><a href="#skada">Skada och avstängning</a></li>
	<li><a href="#uppsagning">Uppsägning</a></li>
<ul>
</div>
{% endsidebar %}

<script>
$( document ).ready(function() {
	$('.navbar li.active').removeClass('active');		    
	$('.navbar li#menu_businessoptions').addClass('active');		
	$('.navbar li#menu_documentation').addClass('active');		    
});
</script>