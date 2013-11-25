---
layout: post
lang: en
title:  "Instructions for Policies"
date:   2013-11-24 9:40:00
---
The API License does not live in a vacuum, instead it is just one delivery needed to publish an API. Among other required items are price lists, documentation etc. The License refers to such documents. These have been separated from the License itself to prevent it to become too large and complicated given the wide array of variants in which e.g. Technical Documentation can be designed.

##<a id="pul">Template: Personal Data Processing Policy</a>
The information which an API provider needs to provide to users who have registered their personal data to gain access to an API depends on what the provider plans to do with the data, but the project recommends that the API provider provide, at a minimum, the following information:

* **Data concerning the identity of the controller of personal data** -  In other words, their name, address, telephone numbers and, where applicable, company registration number and email address. 
* **Data concerning the purpose of the processing** - In other words, a description of why the users are being requested to register their personal data and how the data will be processed.
* **Potential recipients of data** - If the API provider plans to disclose the personal data to a third party (such as a subcontractor, subsidiary or provider of marketing services), the users will be informed which recipients, or categories of recipients, will be entitled to receive the data.
* **The right for registered persons to be informed which data is being processed** - Section 26 of PUL states that a controller of personal data is obliged to inform each person who applies (free of charge and once per calendar year) whether personal data relating to the applicant is being processed or not. An API provider should provide information concerning this right and who the users should contact to exercise such right. 
* **The right for registered persons to have incorrectly processed data corrected, blocked or deleted** - Section 28 of PUL states that a controller of personal data is obliged, at the request of a registered person and as soon as possible, to correct, block or delete incorrectly processed personal data. An API provider should provide information concerning this right and who the users should contact to exercise such right.

##<a id="andring">Template: Modifications Policy</a>
The project recommends that the API provider provide, at a minimum, the following information:

* A description of the various types of technical modifications which can be made to the API (e.g. modifications to the call structure, security-related modifications, etc.), including the differences between the various types of modifications. 
* The manner in which the users will be informed of various planned technical modifications (email, Twitter, notice on the website?)
* The amount of advance notice the users will be given of various planned technical modifications.
* The possibility of sharing the API’s road map, i.e. when new functions are planned to be released also further down the line.
* Where the API provider produces new versions of the API - how long will old versions remain after a new version has been launched?
* The manner in which users will be informed of shutdowns and serious problems.
* The manner in which users will be informed of changes to the terms and conditions of the licence for the API.
* The amount of advance notice the users will be given of planned changes to the terms and conditions of the licence for the API.

###Example wording
We will inform you (as a user) with as much advance notice as possible of any modifications to one of our APIs. Our aim is to inform you as follows: 

* Notice of a major modification to an API will be given at least three months before the modification takes effect, by email to the email address you used to register your account. “Major modification” means a modification which may either disrupt services which use the API or require modifications to the implementation of such services, for example where the API’s interface is modified in a way which results in existing code no longer being compatible. 
* Notice of a minor modification will be given in the API’s documentation no later than the date on which the modification is launched. “Minor modification” means a modification which is not a major modification and which does not affect existing developed services. 
* Emergency modifications (such as due to security problems) will be launched as soon as possible and communicated on our website. We aim to give notice of emergency modifications before a modification is launched, but occasionally we may not be able to provide information concerning an emergency modification until after it has been launched. 
* Notice of any shutdowns or problems in respect of an API will be given by means of a notice on our website and, where we consider it appropriate, by email to the email address you used to register your account.
* Notice that we will be completely removing an existing API will be given at least three months before this takes place by email to the email address you used to register your account.
* Notice of changes to the terms and conditions of the licence will be given by means of publishing a new version of the licence on our website no later than three months before the new version enters into force. 

##<a id="dokumentation">Technical Documentation</a>
Since technical documentation can be drafted in many different ways, no proposals are provided as examples, but the project recommends that the API provider provide, at a minimum, the following information:

* Data format.
* Requirements for keys (if any).
* Technical specification relating to the call structure (question and answer format, frequently asked questions (FAQs)). 
* Information concerning response times and possible ways in which the question can be optimised to allow for shorter response times.
* Possible requirements as to how services which use the API should be structured, including any limitations and/or requirements concerning caching, storage, copying and updates. 
* Any limitations on the number of questions per key/service.
* Information concerning terms and how various terms in the information are defined (metadata).
* Which error messages can be provided and what they mean.
* Available code library.
* Testing possibilities (e.g. API console or testing environment).
* Any possible support from the API provider. 

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Policies</h3>
<ol>	
	<li><a href="#pul">Personal Data Processing Policy</a></li>
	<li><a href="#andring">Modifications Policy</a></li>
	<li><a href="#dokumentation">Technical Documentation</a></li>
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