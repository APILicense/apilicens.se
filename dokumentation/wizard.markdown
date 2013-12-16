---
layout: post
lang: se
title:  "Skräddarsy API-licensen"
date:  2013-12-16 12:39:00
---

<section id="wizard">
<p>Med denna wizard så är det enkelt att gå igenom de vägval som krävs för att skräddarsy API-licensen enligt de exakta rättsliga och affärsmässiga krav som gäller för ett givet API. Dessa val finns även i [textform](/dokumentation/vagval) och det rekommenderas att alla beslut om hur licensen ska skräddarsys görs efter en genomläsning av de [rättsliga](h/dokumentation/rattsligaval) och [affärsmässiga](/dokumentation/affarsval) övervägande som gäller.</p>
<form action="/dokumentation/resultat" method="GET">
  <div id="rootwizard" class="tabbable tabs-left">
    <ul>
      <li> <a href="#tab1" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>1. Skyddat material</a></li>
      <li><a href="#tab2" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>2. Hänvisning till källa</a></li>
      <li><a href="#tab2b" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>3. Varumärke</a></li>
      <li><a href="#tab3" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>4. Personuppgifter</a></li>
      <li><a href="#tab3b" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>5. Lämning av personuppgifter</a></li>
      <li><a href="#tab4" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>6. Tekniska begränsningar</a></li>
      <li><a href="#tab5" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>7. Betalning</a></li>
      <li><a href="#tab6" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>8. Kommersiell användning</a></li>
      <li><a href="#tab7" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>9. Användning till skada</a></li>
      <li><a href="#tab8" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>10. Felrapportering</a></li>
      <li><a href="#tab9" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>11. Ansvar</a></li>
      <li><a href="#tab9b" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>12. Ansvar</a></li>
      <li><a href="#tab10" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>13. Avsluta licens</a></li>
    </ul>
    <div class="tab-content">
      <div class="tab-pane" id="tab1">
        <h3>1. Immaterialrättsligt skyddat material</h3>
        <p>Kommer API:et att lämna ut immaterialrättsligt skyddat material, t.ex. material som omfattas av upphovsrätt eller varumärkesskydd? </p>
        <p><a href="http://apilicens.se/dokumentation/rattsligaval/#immaterialla" class="ext">Läs mer om immaterialla rättigheter</a>.</p>
        <p>
          <label>
            <input type="radio" name="1" value="y" id="1_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="1" value="n" id="1_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab2">
        <h3>2. Hänvisning till källa</h3>
        <p>Ska API-användaren hänvisa till datakällan? </p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#hanvisning" class="ext">Läs mer om att hänvisa till datakällan</a>.</p>
        <p>
          <label>
            <input type="radio" name="2" value="y" id="2_0">
          Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="2" value="n" id="2_1">
            Nej</label>
        </p>
      </div>
         <div class="tab-pane" id="tab2b">
        <h3>3. Varumärke</h3>
        <p>Vill du ha rätt att hänvisa till API-användarens varumärke/firma?</p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#hanvisning" class="ext">Läs mer om att hänvisa till datakällan</a>.</p>
        <p>
          <label>
            <input type="radio" name="3" value="y" id="3_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="3" value="n" id="3_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab3">
        <h3>4. Skydd för personuppgifter</h3>
        <p>Kommer API-användaren att behöva registrera vissa av sina personuppgifter (t.ex. epost-adress eller namn) för att få ta del av API:et? </p>
        <p><a href="http://apilicens.se/dokumentation/rattsligaval/#pul" class="ext">Läs mer om skydd av personuppfigter</a>.</p>
        <p>
          <label>
            <input type="radio" name="4" value="y" id="4_0">
          Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="4" value="n" id="4_1">
            Nej</label>
        </p>
      </div>
         <div class="tab-pane" id="tab3b">
          <h3>5. Skydd för personuppgifter</h3>
        <p>Kommer API:et att lämna ut personuppgifter? </p>
        <p><a href="http://apilicens.se/dokumentation/rattsligaval/#utlamning" class="ext">Läs mer om utlämning av personuppgifter</a>.</p>
        <p>
          <label>
            <input type="radio" name="5" value="y" id="5_0">
          Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="5" value="n" id="5_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab4">
        <h3>6. Tekniska begränsningar i användning av API-innehållet</h3>
        <p>Finns det tekniska begränsningar i hur användaren får använda API-innehållet, t.ex.gällande cachening, lagring, kopiering och uppdatering av API-innehållet? </p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#tekniska" class="ext">Läs mer om tekniska begränsningar</a>.</p>
        <p>
          <label>
            <input type="radio" name="6" value="y" id="6_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="6" value="n" id="6_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab5">
        <h3>7. Betalning för tillgång till API</h3>
        <p>Kommer du att vilja ta betalt för användandet av API:et? </p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#betalning" class="ext">Läs mer om att ta betalt för API-tillgång</a>.</p>
        <p>
          <label>
            <input type="radio" name="7" value="y" id="7_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="7" value="n" id="7_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab6">
        <h3>8. Kommersiell användning av information från API:et</h3>
        <p>Finns begränsningar med avseende på kommersiell användning av information från API:et? </p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#kommersiell" class="ext">Läs mer om kommersiell använding av APIet</a>.</p>
        <p>
          <label>
            <input type="radio" name="8" value="y" id="8_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="8" value="n" id="8_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab7">
        <h3>9. Användning till skada för tillhandahållarens verksamhet</h3>
        <p>Vill du begränsa användningen av API:et för syften som riskerar att skada din verksamhet? </p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#skada" class="ext">Läs mer om skada och avstängning</a>.</p>
        <p>
          <label>
            <input type="radio" name="9" value="y" id="9_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="9" value="n" id="9_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab8">
        <h3>10. Rapportering av fel och brister</h3>
        <p>Ska API:ets användare ha möjlighet att rapportera fel eller brister i den information som hämtas?</p>
        <p>
          <label>
            <input type="radio" name="10" value="y" id="10_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="10" value="n" id="10_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab9">
        <h3>11. Ansvar för fel och brister</h3>
        <p>Lämnas några garantier för informationens kvalitet och korrekthet? </p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#kvalitet" class="ext">Läs mer om kvalitet och korrekthet</a>.</p>
        <p>
          <label>
            <input type="radio" name="11" value="y" id="11_0">
          Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="11" value="n" id="11_1">
            Nej</label>
        </p>
      </div>
         <div class="tab-pane" id="tab9b">
        <h3>12. Ansvar för fel och brister</h3>
        <p>Kommer API-användaren att kunna generera information till API:et?</p>
        <p><a href="http://apilicens.se/dokumentation/affarsval/#kvalitet" class="ext">Läs mer om garantier</a>.</p>
        <p>
          <label>
            <input type="radio" name="12" value="y" id="12_0">
            Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="12" value="n" id="12_1">
            Nej</label>
        </p>
      </div>
      <div class="tab-pane" id="tab10">
        <h3>13. Användarens rätt att avsluta licensen</h3>
        <p>Ska det finnas begränsningar i API-användarens rätt att säga upp licensen?</p>
        <p> <a href="http://apilicens.se/dokumentation/affarsval/#uppsagning" class="ext">Läs mer om att säga upp licensen</a>.</p>
        <p>
          <label>
            <input type="radio" name="13" value="y" id="13_0">
          Ja</label>
        </p>
        <p>
          <label>
            <input type="radio" name="13" value="n" id="13_1">
            Nej</label>
        </p>
      </div>
          <ul class="pager wizard" id="pag">
        <li class="previous first"><a href="#pag">Första</a></li>
        <li class="previous"><a href="#pag">Föregående</a></li>
        <li class="next last" style="display:none;"><a href="#pag">Sista</a></li>
        <li class="next"><a href="#pag">Nästa</a></li>
        <li class="next last finish" style="display:none;">
          <input type="submit" class="btn btn-success" value="Skicka"/>
        </li>
      </ul>
    </div>   
  </div>
</form>
</section>


<script src="/js/jquery.bootstrap.wizard.min.js"></script> 
<script>
	$(document).ready(function() {
		//wizard
	  	$('#rootwizard').bootstrapWizard({
			tabClass: 'nav nav-tabs',
			onTabShow: function(tab, navigation, index) {
			var $total = navigation.find('li').length;
			var $current = index+1;
			var $percent = ($current/$total) * 100;
			$('#rootwizard').find('.bar').css({width:$percent+'%'});
	
			
			// If it's the last tab then hide the last button and show the finish instead
			if($current >= $total) {
				$('#rootwizard').find('.pager .next').hide();
				$('#rootwizard').find('.pager .finish').show();
				$('#rootwizard').find('.pager .finish').removeClass('disabled');
			} else {
				$('#rootwizard').find('.pager .next').show();
				$('#rootwizard').find('.pager .finish').hide();
			}
			if($current == 1) {
				$('#rootwizard').find('.pager .previous').hide();
			} else {
				$('#rootwizard').find('.pager .previous').show();
			}
			
			
		}});

		//validation
		$('input').change(function(){
			$('.tabbable li.active a').addClass('done');
		});

		//links
		$('a.ext').click(function() {
		    $(this).target = "_blank";
		    window.open($(this).prop('href'));
		    return false;
		});
	
	});	
</script>

{% sidebar %}
{% include documentation_sidebar.markdown %}
{% endsidebar %}

<script>
$( document ).ready(function() {
	$('.navbar li.active').removeClass('active');		    
	$('.navbar li#menu_wizard').addClass('active');		
	$('.navbar li#menu_documentation').addClass('active');		    
});
</script>