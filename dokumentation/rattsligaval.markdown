---
layout: post
lang: se
title:  "Rättsliga överväganden"
date:   2013-11-18 13:28:00
---
Den som tillhandahåller ett API behöver ta hänsyn till tvingande lagstiftning. Här presenteras viktiga lagar som kan aktualiseras för ett API, och de vägval som behöver göras på grund av dessa lagar - val som kommer att påverka [licensens utformning](/dokumentation/licens). Eftersom licensen innehåller olika alternativ beroende på de val ett företag gör, är licensen anpassningsbar för många olika användningsfall

En kort version av alla val finns på [snabba vägval](/dokumentation/vagval/).

##<a id="immaterialla">Immateriella rättigheter</a>

###<a id="upphov">Upphovsrättsskydd</a>
Lag (1960:729) om upphovsrätt och konstnärliga verk ger den som har skapat ett litterärt eller konstnärligt verk ensamrätt till att framställa nya exemplar av verket och att göra det tillgängligt för allmänheten, i alla fall som detta sker annat än för rent privat bruk.

Litterära eller konstnärliga verk kan vara t.ex. en text, ett foto, ett datorprogram eller ett musikstycke, förutsatt att texten, fotot, datorprogrammet eller musikstycket är tillräckligt originellt.

Precis som i alla andra fall då ett företag vill dela med sig av material som kan vara upphovsrättsskyddat måste tillhandahållaren av ett API därför kontrollera om API:et returnerar något material som någon annan än tillhandahållaren av API:et har upphovsrätt till, eller som API-tillhandahållaren själv har upphovsrätt till och vill sätta upp begränsningar för användandet av. 

Ett företag som tillhandahåller ett API bör därför undvika att lägga ut bilder, programkod och andra verk i ett API om man inte är säker på att man har fått upphovsmannens rätt att sprida verket vidare på det sätt som görs.

Det händer att rätten att förfoga över ett upphovsrättsligt skyddat verk är villkorad, t.ex. genom att en bild tillhandahålls under en licens som anger att upphovsmannen måste nämnas då bilden kopieras eller sprids. För att förhålla sig till sådana villkor bör en API-tillhandahållare ge användarna (d.v.s. de utvecklare som ges tillgång till API:et) den information de behöver för att inte bryta mot upphovsrätten till något verk, genom att kommunicera de villkor som gäller för de verk som tillhandahålls via API:et. 

Eftersom dessa villkor kommer att variera mellan varje enskilt fall är det inte möjligt att föra in sådana informationstexter i den licenstext som tagits fram inom ramen för projektet, men licenstexten har försetts med utrymme för API-tillhandahållaren att beskriva de ev. villkor som gäller för upphovsrättsskyddat material.

I de fall som användarna själva kan generera information till API:et bör API-tillhandahållaren tydliggöra att användaren själv ansvarar för att han eller hon har rätt att sprida ev. upphovsrättsligt skyddade verk, se [beskrivningen av garantier](/dokumentation/affarsval). 

###<a id="varumarke">Varumärkesskydd</a>
Varumärkeslag (2010:1877) ger den som har registrerat eller inarbetat ett varumärke ensamrätt till att använda varumärket i näringsverksamhet. 

Exempel på varumärkesskyddat material kan vara logotyper, varunamn och symboler, givet att de utgör ett unikt varumärke.

Precis som är fallet med upphovsrättsligt skyddat material har tillhandahållaren av ett API inte rätt att låta sina användare utnyttja ett varumärke som inte tillhör API- tillhandahållaren. Ett företag som tillhandahåller ett API bör därför undvika att lämna ut varumärkesskyddade märken i ett API om man inte är säker på att man har fått innehavarens rätt att låta andra använda varumärket. 

Om API-tillhandahållaren har fått rätten att låta sina användare använda en tredje parts varumärke bör API-tillhandahållaren, liksom är fallet med upphovsrättskyddat material, informerar sina användare om eventuella villkor som gäller för användningen av varumärket. 

Det förekommer också att tillhandahållaren av ett API vill kräva att användaren hänvisar till tillhandahållarens eget varumärke eller firma i samband med att användaren publicerar information som användaren fått tillgång till via API:et. 

Vissa tillhandahållare av API:er vill också själva ha rätt att ange användarens varumärke eller firma för att annonsera vem som använder sig av API:et. Varumärkesanvändningen i sådana situationer behandlas i punkt 5.4 nedan.

####Vägval i licensen
Kommer API:et att lämna ut immaterialrättsligt skyddat material, t.ex. material som omfattas av upphovsrätt eller varumärkesskydd?	

* Ja: Behåll [punkt 2.2 i licenstexten](/dokumentation/licens#2.2) och infoga efterfrågad information.
* Nej: Stryk [punkt 2.2 i licenstexten](/dokumentation/licens#2.2)

##<a id="pul">Skydd för personuppgifter</a>

### Bakgrund
Personuppgiftslag (1998:204) (PUL) anger förutsättningarna för automatiserad behandling av personuppgifter i verksamhet som inte är av rent privat natur. 

I PUL definieras personuppgifter som ”all slags information som direkt eller indirekt kan hänföras till en fysisk person som är i livet”, vilket t.ex. kan vara:

* En fysisk persons namn
* En fysisk persons e-postadress
* IP-nummer som kan kopplas till en fysisk person
* Användarnamn i sociala nätverk.

Med behandling avses i princip varje åtgärd som vidtas med en personuppgift, t.ex. insamling, registrering, organisering, lagring, bearbetning, ändring, användning, utlämnande genom översändande, spridning, sammanställning, blockering, eller utplåning.

Bestämmelserna i PUL riktar sig mot den personuppgiftsansvarige, d.v.s. den enhet som ensam eller tillsammans med andra bestämmer ändamålen med och medlen för behandlingen personuppgifter. I PUL uppställs en rad krav på den personuppgiftsansvarige, t.ex. 

* krav på viss information till de registrerade;
* krav på att vidta lämpliga tekniska och organisatoriska åtgärder för att skydda de personuppgifter som behandlas;
* krav på att den personuppgiftsansvarige inte får överföra personuppgifter till ett tredje land (d.v.s. ett land utanför EU/EES) utan rättslig grund.

###<a id="inhamtande">Inhämtande av personuppgifter</a>
Många API-tillhandahållare kräver att en användare registrerar viss information om sig själv (t.ex. namn och e-postadress) för att få tillgång till API:et. API-tillhandahållaren blir att betrakta som personuppgiftsansvarig för de personuppgifter som samlas in på det här sättet, och måste då förhålla sig till PUL:s krav på en personuppgiftsansvarig. 

Flera av dessa krav faller utanför ramen för projektet, men för att ge en fingervisning om vilken information en personuppgiftsansvarig bör lämna till de registrerade (d.v.s. till användare som har registrerat sina uppgifter för att få tillgång till ett API) innehåller licensen en hänvisning till en policy för personuppgiftshantering. Projektet rekommenderar att en API-tillhandahållare lämnar åtminstone den information som framgår av mallen för Policy för Personuppgiftsbehandling. 

####Vägval i licensen
Kommer API-användaren att behöva registrera vissa personuppgifter (t.ex. e-postadress eller namn) för att få ta del av API:et? 	

* Ja: Behåll [punkt 3.1 i licenstexten](/dokumentation/licens#3.1).
* Nej: Stryk [punkt 3.1 i licenstexten](/dokumentation/licens#3.1)

###<a id="utlamning">Utlämning av personuppgifter</a>
När ett företag vill lämna ut information som innehåller personuppgifter genom ett API är utgångspunkten normalt sett att företaget är personuppgiftsansvarigt enligt PUL, och att utlämnandet av uppgifterna är att betrakta som en behandling av personuppgifterna.

Av PUL framgår att varje behandling (t.ex. ett utlämnande till API-användare) kräver en laglig grund, vilket antingen kan bestå i att den personuppgiftsansvarige har fått den registrerade personens samtycke till behandlingen, eller att behandlingen är nödvändig för att kunna fullgöra ett avtal med den registrerade, för att den personuppgiftsansvarige ska kunna fullgöra en rättslig skyldighet eller dyl. (se § 10 PUL).

När ett API ska lanseras måste tillhandahållaren därför, i ett första steg, kontrollera om det förekommer några personuppgifter i den information som ska lämnas ut. Om så är fallet måste tillhandahållaren kontrollera att man har laglig grund att lämna ut uppgifterna till API-användarna, t.ex. genom att man har fått de registrerades samtycke till att göra detta. 

Eftersom de API-användare som tar del av personuppgifterna i sin tur kommer att bli personuppgiftsansvariga för sin behandling av uppgifterna rekommenderar projektet att API-tillhandahållaren informerar användarna om att de måste se till att deras egen behandling av personuppgifter sker i enlighet med PUL. 

I de fall som användare själva kan generera information till ett API bör API-tillhandahållaren tydliggöra att användaren själv ansvarar för att han eller hon har rätt att sprida ev. personuppgifter som tillgängliggörs av användaren i API:et, se [beskrivningen av garantier](/dokumentation/affarsval). 

###Vägval i licensen
Kommer API:et att lämna ut personuppgifter?	

* Ja: Behåll [punkt 3.2 i licenstexten](/dokumentation/licens#3.2).
* Nej: Stryk [punkt 3.2 i licenstexten](/dokumentation/licens#3.2)

##<a id="aterskapa">Krav att licensen ska kunna återskapas</a>
Lag (2002:562) om elektronisk handel och andra informationssamhällets tjänster (”E-handelslagen”) innehåller ett antal krav på vilken information som en tillhandahållare av ”informationssamhällets tjänster” ska lämna till sina användare.

Som framgår av de begränsningar som har uppställts för projektet har vi gjort bedömningen att stora delar av dessa informationskrav inte behöver uppfyllas i själva licenstexten, utan istället kan anges på andra delar av den webbplats där ett API tillhandahålls. 

Av § 13 E-handelslagen framgår emellertid ett krav på att ”avtalsvillkor ska göras tillgängliga för tjänstemottagare på ett sätt som gör det möjligt att spara och återskapa dem”.

Projektet rekommenderar därför att API-tillhandahållare tillhandahåller sin licenstext i ett publikt versionshanteringssystem (t.ex. [GitHub](https://github.com)), i pdf-format eller ett motsvarande format som gör det möjligt för API-användare att spara och återskapa den. 

I de fall som en API-tillhandahållare har ändrat något villkor i sin licenstext bör företaget publicera en ny version av licensen i ett format som kan sparas och återskapas av användarna. Angående kommunikation till användare om förändringar i licenstexten, se vidare punkt 5.6 nedan.

###Implikation för licensen
Se [punkt 7.2 i licenstexten](/dokumentation/licens#7.2).


{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Rättsliga överväganden</h3>
<ul>
	<li><a href="#immaterialla">Immateriella rättigheter</a></li>
	<li><a href="#upphov">Upphovsrättsskydd</a></li>
	<li><a href="#varumarke">Varumärkesskydd</a></li>
	<li><a href="#pul">Skydd för personuppgifter</a></li>
	<li><a href="#inhamtande">Inhämtande av personuppgifter</a></li>
	<li><a href="#utlamning">Utlämning av personuppgifter</a></li>
	<li><a href="#aterskapa">Krav att licensen ska kunna återskapas</a></li>	
<ul>
</div>
{% endsidebar %}

<script>
$( document ).ready(function() {
	$('.navbar li.active').removeClass('active');		    
	$('.navbar li#menu_legaloptions').addClass('active');		
	$('.navbar li#menu_documentation').addClass('active');		    
});
</script>