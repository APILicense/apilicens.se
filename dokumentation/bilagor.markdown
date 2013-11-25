---
layout: post
lang: se
title:  "Instruktioner för bilagor"
date:   2013-11-21 12:47:00
---
API-licensen lever inte i ett vacuum utan är bara en del av allt som måste finnas på plats när ett API levereras. Det krävs även ev. prislistor, dokumentation och mycket annat. Licensen hänvisar till en del sådana dokument, som har separerats från licensen för att inte göra licensen alltför stor och svårhanterlig. 

##<a id="pul">Mall: Policy för personuppgiftsbehandling</a>
Vilken information en API-tillhandahållare behöver lämna till användare som har registrerat sina personuppgifter för att få tillgång till ett API beror på vad tillhandahållaren planerar att göra med uppgifterna, men projektet rekommenderar att API- tillhandahållaren lämnar åtminstone följande information:

* **Uppgifter om den personuppgiftsansvariges identitet** - D.v.s. uppgift om namn, adress, telefonnummer och i förekommande fall organisationsnummer och e-postadress. 
* **Uppgifter om ändamålet med behandlingen** - D.v.s. en beskrivning av varför man ber användarna att registrera sina personuppgifter och hur man planerar att behandla uppgifterna.
* **Eventuella mottagare av uppgifter** - Om API-tillhandahållaren planerar att lämna ut personuppgifterna till en tredje part (såsom underleverantörer, dotterbolag eller leverantörer av marknadsföringstjänster) ska användarna informeras om vilka mottagare, eller kategorier av mottagare, som kan få del av uppgifterna. 
* **De registrerades rätt att få information om vilka uppgifter som behandlas** - Av 26 § PUL följer att en personuppgiftsansvarig är skyldig att till var och en som ansöker om det en gång per kalenderår gratis lämna besked om personuppgifter som rör den sökande behandlas eller inte. En API-tillhandahållare bör informera om den här rätten, och vart användarna ska vända sig för att utnyttja den. 
* **De registrerades rätt att få felaktigt behandlade uppgifter rättade, blockerade eller utplånade** - Av 28 § PUL följer att en personuppgiftsansvarig är skyldig att på begäran av den registrerade snarast rätta, blockera eller utplåna felaktigt behandlade personuppgifter. En API-tillhandahållare bör informera om den här rätten och vart användarna ska vända sig för att utnyttja den.

##<a id="andring">Mall: Policy för ändringshantering</a>
Projektet rekommenderar att API- tillhandahållaren lämnar åtminstone följande information:

* En beskrivning av de olika typer av tekniska förändringar av API:et som man kan komma att genomföra (t.ex. ändringar i anropsstruktur, säkerhetsrelaterade ändringar etc.), inkl. skillnaderna mellan dessa olika typer. 
* Hur användarna informeras om olika planerade tekniska förändringar (mail, Twitter, meddelande på hemsida?)
* Hur lång tid i förväg användarna informeras om olika planerade tekniska förändringar.
* Eventuellt dela med sig av API:ets road map, d.v.s. när nya funktioner är planerade att släppas även längre in i framtiden.
* I den mån man arbetar med versionshantering av API:et- Hur länge finns gamla versioner kvar efter att en ny version lanserats?
* Hur användaren informeras om driftstörningar och akuta problem.
* Hur användarna informeras om förändringar i API:ets licensvillkor.
* Hur lång tid i förväg användarna informeras om planerade förändringar i API:ets licensvillkor.

###Exempeltext
Vid förändringar i ett av våra API:er kommer vi att informera dig som användare med så god varsel som möjligt. Vår ambition är att informera dig som användare enligt följande: 

* Information om en större förändring i ett API lämnas minst tre månader innan förändringen träder i kraft, genom epost till den mailadress som du har använt för att registrera ditt konto. Med en större förändring menar vi en förändring som antingen kan komma att störa tjänster som använder sig av API:et eller som kan komma att kräva ändringar i sådana tjänsters implementering. 
* Information om en mindre förändring meddelas i API:ets dokumentation senast i anslutning till driftsättning av förändringen. Med en mindre förändring menar vi alla förändringar som inte är större förändringar. 
* Akuta förändringar (till exempel till följd av säkerhetsproblem) driftsätts snarast möjligt och kommuniceras på vår webbplats. Vi strävar efter att lämna information om akuta förändringar innan en sådan förändring driftsätts, men det kan hända att vi inte har möjlighet att gå ut med information om en akut förändring förrän i efterhand. 
* Information om eventuella driftstörningar eller problem i ett API kommuniceras genom meddelanden på vår webbplats och, i de fall som vi bedömer att det är lämpligt, genom e-post till den mailadress som du har använt för att registrera ditt konto.
* Information om att vi helt kommer att ta bort ett befintligt API lämnas minst tre månader innan så sker, genom epost till den mailadress som du har använt för att registrera ditt konto.
* Information om förändringar i licensvillkor kommuniceras genom att en ny version av licenstexten publiceras på vår webbplats senast tre månader innan den nya versionen träder i kraft. 

##<a id="dokumentation">Teknisk dokumentation</a>
Då teknisk dokumentation kan utformas på många sätt ges inget förslag på exempel med projektet rekommenderar att API- tillhandahållaren lämnar åtminstone följande information:

* Dataformat.
* Eventuella krav på nycklar.
* Teknisk specifikation kring anropsstruktur (format för fråga och svar, exempelfrågor).  
* Information om responstider och eventuella sätt som frågan kan optimeras för att ge kortare responstider.
* Eventuella krav på hur tjänster som använder API:et ska utformas, inklusive eventuella begränsningar och/eller krav avseende cachening, lagring, kopiering och uppdatering. 
* Eventuella begränsningar i antal frågor per nyckel/tjänst.
* Information kring begrepp och hur olika begrepp i informationen definieras (metadata).
* Vilka felmeddelanden som kan lämnas och vad de innebär.
* Tillgängliga kodbibliotek.
* Testmöjligheter (t.ex. API-konsol eller testmiljö).
* Eventuella möjligheter till support från API-tillhandahållaren. 

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Bilagor</h3>
<ol>	
	<li><a href="#pul">Policy för personuppgiftsbehandling</a></li>
	<li><a href="#andring">Policy för ändringshantering</a></li>
	<li><a href="#dokumentation">Teknisk dokumentation</a></li>
<ol>
</div>
{% endsidebar %}

<script>
$( document ).ready(function() {
	$('.navbar li.active').removeClass('active');		    
	$('.navbar li#menu_attachments').addClass('active');		
	$('.navbar li#menu_documentation').addClass('active');		    
});
</script>