---
layout: post
lang: en
title:  "API Terms of License - results from wizard"
date:   2013-12-14 06:23:00
---
<script>
$( document ).ready(function() {

	var hideShowOptions = function(n){
		if ($.url().param(n) == "n") {
			$('.choice'+n+'y').parent('li').remove(); //Remove list item in the "left to do" list
			$('.choice'+n+'y').remove();
			$('.choice'+n).remove();
			$('#response'+n).html('No');
		}
		else if ($.url().param(n) == "y") {
			$('.choice'+n+'n').parent('li').remove();
		 	$('.choice'+n+'n').remove();
			$('.choice'+n).remove();
		}	
		else {
			$('#response'+n).html('No choice made');	
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

The License below is based on the following [choices](/en/dokumentation/wizard):

* Will the API distribute any content protected by intellectual property rights? - **<span id="response1">Yes</span>**
* Should the API-user refer to the data source?  - **<span id="response2">Yes</span>**
* Do you want have the right to refer to the API-user’s trademark/trade name? - **<span id="response3">Yes</span>**
* Will the API-user need to register any personal data to be able to connect to the API? - **<span id="response4">Yes</span>**
* Will the API disclose any personal data? - **<span id="response5">Yes</span>**
* Are there any technical limitations as regards how the user may use the API-content? - **<span id="response6">Yes</span>**
* Do you want to charge for the use of the API? - **<span id="response7">Yes</span>**
* Are there any limitations as regards commercial use of the information in the API? - **<span id="response8">Yes</span>**
* Do you want to exclude use of the API for purposes which may harm your business? - **<span id="response9">Yes</span>**
* Should the API-user be able to report errors or defects in the accessed information? - **<span id="response10">Yes</span>**
* Are you willing to provide any warranties regarding the quality/accuracy of the information? - **<span id="response11">Yes</span>**
* Will the API-user be able to generate information to the API? - **<span id="response12">Yes</span>**
* Should there be any limitations to the API-user’s right to terminate the licence?  - **<span id="response13">Yes</span>**

Left to do:

* **<a href="#0">Background</a>** - Inserts API provider's name and website, also replace *Name* in the rest of the License with the provider's name
* <span class="choice1y">**<a href="#2.2">2.2</a>** - Insert about intellectual property rights and license terms for API content</span>
* <span class="choice2y">**<a href="#2.3">2.3</a>** - Insert description of the method of reference</span>
* <span class="choice4y">**<a href="#3.1">3.1</a>** - Insert link to Personal Data Processing Policy</span>
* <span class="choice6y">**<a href="#4.1">4.1</a>** - Insert link to Technical Documentation and update the list of technical limitations</span>
* <span class="choice7y">**<a href="#5.2">5.2</a>** - Insert link to the Price List</span>
* <span class="choice9y">**<a href="#5.4">5.4</a>** - Insert description of what may harm the provider’s interests.</span>
* <span class="choice10y">**<a href="#6.1">6.1</a>** - Insert e-mail address where errors should be reported</span>
* <span class="choice11y">**<a href="#6.2">6.2</a>** - Insert description of warranty</span>
* <span class="choice11n">**<a href="#6.2">6.2</a>** - Insert link to Technical Documentation and to the Change Management Policy</span>
* **<a href="#7.1">7.1</a>** - Insert link to the Change Management Policy
* **<a href="#8.2">8.2</a>** - Insert link to the Change Management Policy
* <span class="choice13y">**<a href="#8.3">8.3</a>** - Insert notice period and methods of termination etc</span>
* <span class="choice13n">**<a href="#8.3">8.3</a>** - Insert description of how to discontinue use of the API</span>

##<a id="0">Background</a>
[*Insert provider’s name*]&nbsp;(”[**Name**]”) provides an API (the ”**API**”) on the website [Insert websites], which provides you access to information, code and other material (the ”**API-content**”). 

These terms of licence (the “**Agreement**”) describe under what conditions the API is provided, how you are expected to use the API and what your rights and obligations are when using the API-content in your own products or services.

By accepting the terms of this Agreement you certify that you have read, understood and accept the terms set out herein and in the documents referred to in this Agreement. 

##<a id="1">1. License</a>
[*Name*] hereby grants you a non-exclusive, non-assignable, non- transferable and revocable licence to use the API in accordance with this Agreement. This licence, and the products and services which you develop under the licence, do not constitute any limitation in [*Name*]’s or our data sources’ right to freely use, develop, amend and to stop providing the API, the API-content and related products and services.

As further set out below, we will keep you updated on changes to the API and our ability to provide the API.

##<a id="2">2. Intellectual Property Rights</a>
**<a id="2.1">2.1</a>** [*Name*] and/or the third parties with which we are cooperating hold the ownership and the intellectual property rights to the API. Unless you have received our express written consent you are not entitled to claim the ownership of, publish, copy, assign, transfer, license or otherwise dispose of the intellectual property rights to the source code or call structure of the API.

<span class="choice1y">**<a id="2.2">2.2</a>** The API-content includes content which is protected by intellectual property rights, such as copyright and trademark protection and you are not entitled to claim ownership of, publish, copy, assign, transfer, license or amend such content other than in accordance with the applicable licence terms for each work.][*Insert information on how the API-user can receive information on which API-content is protected by intellectual property rights and which licence terms are applicable for such content, for example by referring to the applicable Creative Commons-licence.*</span>

**<a id="2.3">2.3</a>** <span class="choice2y">When using the API-content in products or services developed by you, you are obliged to indicate, in the product or service at hand, that it contains data from the API and to refer to the API by [*insert description of the method of reference*]. Your right to use [*Name*]’s trade name and trademark is limited to source references in accordance with the aforesaid, and you are not entitled to use our trade name or our trademarks other than set out in this section. </span><span class="choice2n">When using the API-content in products or services developed by you, you are not entitled to refer to the API or to [*Name*]’s trade name or trademark.</span>

<span class="choice3y">**<a id="2.4">2.4</a>** By submitting requests to the API, you grant [*Name*] a non-exclusive, non-assignable  and non- transferable licence to refer to your trade name and any products and services in which the API-content is used (including any trademarks which you hold for such products or services), for the purpose of indicating that you are using the API. [*Name*]’s right to use your trade name and trademark is limited to source references for this purpose.</span>

##<a id="3">3. Processing of Personal Data</a>
<span class="choice4y">**<a id="3.1">3.1</a>** In order to be able to submit request to the API, you may need to register certain personal data pertaining to you. By registering your personal data, you accept that [*Name*] processes your personal data for the purpose of administrating, supervising and enabling your use of the API, and that [*Name*], acting as a data controller in accordance with the Personal Data Act (Personuppgiftslag (1998:204)), processes your personal data in accordance with our Policy for processing of personal data [*Insert link to Policy*. </span>

<span class="choice5y">**<a id="3.2">3.2</a>** The API-content includes personal data, and you are aware and accept that by collecting, using, aligning, compiling or otherwise processing such personal data you are acting as a data controller for the processing in accordance with the Personal Data Act (*Personuppgiftslag (1998:204))*.</span>

##<a id="4">4. Technical Requirements and Limitations</a>
<span class="choice6y">**<a id="4.1">4.1</a>** For the purpose of securing and maintaining the availability and quality of the API and the API-content you are obliged to adhere to our instructions regarding [*caching, storing, copying and updating*] the API-content, as set out in our Technical Documentation [*Insert link to Technical Documentation*.</span>

**<a id="4.2">4.2</a>** You may only connect to the API in the way set out in our instructions and you are not entitled to use any technical means to gain unauthorized access to, disturb or deactivate the API. This includes, but is not limited to, that you undertake not to introduce viruses, worms, Trojan horses or other forms of malware in the API or on the website where the API is provided. 

##<a id="5">5. Other Requirements of Use</a>
**<a id="5.1">5.1</a>** You have to be 18 years of age to enter into this Agreement and to access the API.

<span class="choice7y">**<a id="5.2">5.2</a>** Your access to the API and the API-content is subject to your payment of charges, in accordance with the prices and terms of payment set out in our Price List [*Insert link to the Price List*].</span>

<span class="choice8y">**<a id="5.3">5.3</a>** [**Alt. 1**: You are not entitled to use the API-content for any commercial purpose. This means that you are not entitled to use the API-content in a product or service which in any way generates income, including but not limited to by means of financing through advertising or by requiring payment for membership or subscription.]</span>

<span class="choice8y">[**Alt.2**: Your right to use the API-content for commercial purposes is limited, to the extent that you are not entitled to charge users for the products or services in which you use the API-content. You are however entitled to use the API-content for products or services which are financed by advertising.]</span>

<span class="choice9y">**<a id="5.4">5.4</a>** You are not entitled to use the API or the API-content for products and services which may harm [*Name*]’s business or which violates our interests. This means that the API and the API-content may not be used for products or services which [*insert description of products/services/contexts which may harm the provider’s interests.*]</span>

**<a id="5.5">5.5</a>** You are not entitled to use the API or the API-content for products or services which are in breach of or which allude to the breach of applicable laws and regulations.

**<a id="5.6">5.6</a>** If you have any questions regarding the limitations set out in this section ”Other requirements of use” or if you wish to use the API or the API-content in any other way than as set out in this section, you may contact us at [*insert e-mail address*]. You are however not entitled to commence such use before you have received our written consent. 

##<a id="6">6. Liability</a>
<span class="choice10y">**<a id="6.1">6.1</a>** We strive to constantly improve the API and welcome you to inform us of any errors or defects in your user experience by sending us a message at [*insert e-mail address*]. As further specified in this section ”Liability” we however have limited possibilities to correct errors or defects.</span>

**<a id="6.2">6.2</a>** <span class="choice11y">We provide the following, limited warranty for the API and the API-content: [*insert description of warranty.*].Otherwise, you accept that [*Name*] does not commit to, or provide any warranties regarding the API’s or the API-content’s quality, security, reliability, availability or performance.</span><span class="choice11n">You are aware and accept that [*Name*] does not commit to, or provide any warranties regarding the quality, security, reliability, availability or performance of the API or the API-content. Accordingly, notwithstanding what is set out in our Technical Documentation [*Insert link to the Technical Documentation*], Policy for Change Management [*Insert link to the Policy*] or other descriptions of the API’s function where the API is provided, you cannot expect that the API is error free, free from security issues, updated, or a suitable data source for the products or services you intend to use the API for.</span>

**<a id="6.3">6.3</a>** You are aware and accept that you use the API at your own risk and that [*Name*] is not liable for any indirect damage which you may suffer due to your use of, respectively your inability to use, the API or the API-content. In this Agreement, indirect damage shall be interpreted to mean for example loss of profit, loss of use of your products or services, reimbursement for the use of a replacing service, loss of data, costs for trouble shooting, loss of goodwill and damage due to viruses and other security related issues. You also accept that [*Name*]’s total liability for damages due to your use of, respectively your inability to use, the API and the API-content is limited to [*insert sum*].

<span class="choice12y">**<a id="6.4">6.4</a>** By generating data and information to the API, you accept that you are responsible for your right to publish and distribute such information, including but not limited to a responsibility to ensure that you (i) do not violate any third party’s intellectual property rights, (ii) are entitled to distribute any personal data, (iii) do not distribute information in breach of, or which allude to the breach of, applicable laws and regulations.</span>

**<a id="6.5">6.5</a>** You undertake to indemnify [*Name*], our partners and employees against any claims from third parties pertaining to your use of the API or the API-content in breach of this Agreement.

##<a id="7">7. Changes</a>
**<a id="7.1">7.1</a>** We reserve the right to update and change the API, the API-content and this Agreement in accordance with our Change Policy [*Insert link to Policy*]. The change policy sets out which changes may occur, how changes are communicated to you and how long in advance. 

**<a id="7.2">7.2</a>** Changes to this Agreement are documented by the issuance of a new version of these terms. Each new version will be provided with a new version number, set out at the end of the document. 

**<a id="7.3">7.3</a>** By continuing to use the API after a change has been executed, out you confirm that you accept the change. If you do not accept a change you are no longer entitled to use the API and must discontinue your connection to the API in accordance with the section ”Term and Termination” below.

##<a id="8">8. Terms and Conditions</a>
**<a id="8.1">8.1</a>** This Agreement, and your licence to the API, enters into force when you accept this Agreement, and remains in force as long as [*Name*] provides the API, unless previously terminated in accordance with this section “Term and Termination”.

**<a id="8.2">8.2</a>** [*Name*] reserves the right to immediately terminate this Agreement and to discontinue your use of the API if you use the API or the API-content in breach of the provisions set out herein. We also reserve the right to, based on our reasonable assessment and following notice to you, in accordance with our Change Policy [*Insert link to Policy*], permanently or temporarily discontinue the API or the API-content in part or in its entirety.

**<a id="8.3">8.3</a>** <span class="choice13y">You are entitled to terminate this Agreement, provided that you [*insert notice period, method of termination and any applicable charge for early termination*]</span><span class="choice13n">You are entitled to at any time, without grounds and without cost terminate this Agreement. Such termination is carried out by discontinuing your use of the API by [*insert description of how to discontinue use of the API.*].</span>

**<a id="8.4">8.4</a>** If your right to use the API is terminated, you are liable to immediately discontinue and erase your connection to the API<span class="choice2y"> and any references to our trade name and our trademarks used in your products or services</span>.

##<a id="9">9. Miscellaneous</a>
**<a id="9.1">9.1</a>** This Agreement constitutes the entire agreement on all matters concerning your right to use the API and the API-content. Changes in or amendments to this Agreement other than new versions in accordance with the section ”Changes” above shall, in order to be valid, be carried out by way of written confirmation from [*Name*].

**<a id="9.2">9.2</a>** You are not entitled to transfer your rights and obligations under this Agreement to a third party. [*Name*] reserves the right to, after notice to you, assign the Agreement to any of our group companies or to a third party which acquire our business, in part or in its entirety.

**<a id="9.3">9.3</a>** If and to the extent that any of your obligations, or any limitation of your rights in accordance with this Agreement, are not valid because of your rights as a consumer, they shall not be applicable to you. Accordingly, nothing in this Agreement is intended to exclude or limit your lawful rights as a consumer.

**<a id="9.4 ">9.4</a>** This Agreement shall be governed by and construed in accordance with the laws of Sweden. Any disputes which arise in relation to this Agreement shall be settled in Swedish courts.

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>The License</h3>
<ol>	
	<li><a href="#1">License</a></li>
	<li><a href="#2">Intellectual Property Rights</a></li>
	<li><a href="#3">Processing of Personal Data</a></li>
	<li><a href="#4">Technical Requirements and Limitations</a></li>
	<li><a href="#5">Other Requirements of Use</a></li>
	<li><a href="#6">Liability</a></li>
	<li><a href="#7">Changes</a></li>
	<li><a href="#8">Term and Termination</a></li>
	<li><a href="#9">Miscellaneous</a></li>
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