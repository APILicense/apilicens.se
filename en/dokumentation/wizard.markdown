---
layout: post
lang: en
title:  "API License Wizard"
date:  2013-12-16 12:57:00
---

<section id="wizard">
<p>This wizard makes easy to walk through all the choices needed to customise the License accroding to the legal and commercial considerations required for a particular API. These choices are also available as [text](/en/dokumentation/vagval) and it is recommended that all decisions made about the License customisation are made after the [legal](/rn/dokumentation/rattsligaval) and [commercial](/en/dokumentation/affarsval) options are studied.</p>
<form action="/en/dokumentation/resultat" method="GET">
  <div id="rootwizard" class="tabbable tabs-left">
      <ul>
        <li> <a href="#tab1" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>1. IP rights</a></li>
        <li><a href="#tab2" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>2. Source reference</a></li>
        <li><a href="#tab2b" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>3. User trademark</a></li>
        <li><a href="#tab3" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>4. Personal data</a></li>
        <li><a href="#tab3b" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>5. Disclosure of Personal Data</a></li>
        <li><a href="#tab4" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>6. Technical limitations</a></li>
        <li><a href="#tab5" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>7. Payment</a></li>
        <li><a href="#tab6" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>8. Commercial use</a></li>
        <li><a href="#tab7" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>9. Harmful use</a></li>
        <li><a href="#tab8" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>10. Error reporting</a></li>
        <li><a href="#tab9" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>11. Liability</a></li>
        <li><a href="#tab9b" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>12. Liability</a></li>
        <li><a href="#tab10" data-toggle="tab"><span class="glyphicon glyphicon-ok-sign"></span>13. Termination</a></li>
      </ul>
      <div class="tab-content">
        <div class="tab-pane" id="tab1">
          <h3>1. Content protected by intellectual property rights</h3>
          <p>Will the API distribute any content protected by intellectual property rights, e.g. copyrighted content or content protected by trademark?</p>
          <p><a href="http://apilicens.se/en/dokumentation/rattsligaval/#immaterialla" class="ext">Read more about Intellectual Property Rights</a>.</p>
          <p>
            <label>
              <input type="radio" name="1" value="y" id="1_0">
              Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="1" value="n" id="1_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab2">
          <h3>2. Source reference</h3>
          <p>Should the API-user refer to the data source? </p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#hanvisning" class="ext">Read more about referencing the source</a>.</p>
          <p>
            <label>
              <input type="radio" name="2" value="y" id="2_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="2" value="n" id="2_1">
              No</label>
          </p>
        </div>
           <div class="tab-pane" id="tab2b">
          <h3>3. Users' trademark</h3>
          <p>Do you want have the right to refer to the API-user&rsquo;s trademark/trade name?</p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#hanvisning" class="ext">Read more about referencing the source</a>.</p>
          <p>
            <label>
              <input type="radio" name="3" value="y" id="3_0">
              Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="3" value="n" id="3_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab3">
          <h3>4. Protection of personal data</h3>
          <p>Will the API-user need to register any personal data (for example e-mail address or name) to be able to connect to the API? </p>
          <p><a href="http://apilicens.se/en/dokumentation/rattsligaval/#pul" class="ext">Read more about the Protection of Personal Data</a>.</p>
          <p>
            <label>
              <input type="radio" name="4" value="y" id="4_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="4" value="n" id="4_1">
              No</label>
          </p>
        </div>
           <div class="tab-pane" id="tab3b">
            <h3>5. Protection of personal data</h3>
          <p>Will the API disclose any personal data? </p>
          <p><a href="http://apilicens.se/en/dokumentation/rattsligaval/#utlamning" class="ext">Read more about the disclosure of personal data</a>.                </p>
          <p>
            <label>
              <input type="radio" name="5" value="y" id="5_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="5" value="n" id="5_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab4">
          <h3>6. Technical limitations when using the API-content</h3>
          <p>Are there any technical limitations as regards how the user may use the API-content, for example concerning caching, storing, copying and updating the API-content? </p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#tekniska" class="ext">Read more about technical limitations</a>.</p>
          <p>
            <label>
              <input type="radio" name="6" value="y" id="6_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="6" value="n" id="6_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab5">
          <h3>7. Payment for access to the API</h3>
          <p>Do you want to charge for the use of the API?                </p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#betalning" class="ext">Read more about charging for the API</a>.</p>
          <p>
            <label>
              <input type="radio" name="7" value="y" id="7_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="7" value="n" id="7_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab6">
          <h3>8. Commercial use of information in the API</h3>
          <p>Are there any limitations as regards commercial use of the information in the API? </p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#kommersiell" class="ext">Read more about commercial use of the information in the API</a>.</p>
          <p>
            <label>
              <input type="radio" name="8" value="y" id="8_0">
              Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="8" value="n" id="8_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab7">
          <h3>9. Harmful use</h3>
          <p>Do you want to exclude use of the API for purposes which may harm your business? </p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#skada" class="ext">Read more about harmful use</a>.</p>
          <p>
            <label>
              <input type="radio" name="9" value="y" id="9_0">
              Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="9" value="n" id="9_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab8">
          <h3>10. Reporting errors and defects</h3>
          <p>Should the API-user be able to report errors or defects in the accessed information?</p>
          <p>
            <label>
              <input type="radio" name="10" value="y" id="10_0">
              Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="10" value="n" id="10_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab9">
          <h3>11. Liability for errors and defects</h3>
          <p>Are you willing to provide any warranties as regards the quality and accuracy of the information? </p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#kvalitet" class="ext">                Read more about liability for errors and defects</a>.</p>
          <p>
            <label>
              <input type="radio" name="11" value="y" id="11_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="11" value="n" id="11_1">
              No</label>
          </p>
        </div>
           <div class="tab-pane" id="tab9b">
          <h3>12. Liability for generated information</h3>
          <p>Will the API-user be able to generate information to the API?</p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#kvalitet" class="ext">Read more about liability for errors and defects</a>.</p>
          <p>
            <label>
              <input type="radio" name="12" value="y" id="12_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="12" value="n" id="12_1">
              No</label>
          </p>
        </div>
        <div class="tab-pane" id="tab10">
          <h3>13. User’s right to terminate the licence</h3>
          <p>Should there be any limitations to the API-user&rsquo;s right to terminate the licence? </p>
          <p><a href="http://apilicens.se/en/dokumentation/affarsval/#uppsagning" class="ext">Read more about terminating the license</a>.</p>
          <p>
            <label>
              <input type="radio" name="13" value="y" id="13_0">
            Yes</label>
          </p>
          <p>
            <label>
              <input type="radio" name="13" value="n" id="13_1">
              No</label>
          </p>
        </div>
            <ul class="pager wizard" id="pag">
          <li class="previous first"><a href="#pag">First</a></li>
          <li class="previous"><a href="#pag">Previous</a></li>
          <li class="next last" style="display:none;"><a href="#pag">Last</a></li>
          <li class="next"><a href="#pag">Next</a></li>
          <li class="next last finish" style="display:none;">
            <input type="submit" class="btn btn-success"/>
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