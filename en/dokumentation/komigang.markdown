---
layout: post
lang: en
title:  "Get Started with the License"
date:   2013-11-21 16:45:00
---
If you need a user agreement for an API then follow these steps...

##1. Is this the right license?
To make sure that the license fits your API please read through the [Limitations of the License](/en/dokumentation/begransningar) and the [Terms & Conditions](/en/dokumentation/villkor) that applies. In summary the License is designed for companies that publishes web based APIs and that require that each API user actively approves the License. 

Note that the License itself is based on Swedish Law. Nonetheless, we velieve all supporting documentation (such as the [Legal](/en/dokumentation/rattsligaval) and [Commercial Options](/en/dokumentation/affarsval)) should be of value to anyone writing an API License.

##2. Customize the License
The License is designed to be flexible enough to fit many different use cases. To determine which paragraphs in the License that should be used in a particular case please go through all the possible [legal and commercial options](/en/dokumentation/wizard). 

Depending on which options that are chosen there might be a need for additional information to be inserted into the [License itself](/dokumentation/licens/). Such information is [*written in italics*] in the body of the License. Based on the choices made there might also be a need for additional [policy documents](/en/dokumenation/bilagor/) containing additional custom information.

When all choices have been made and all additional information is provided the License is ready to be used, unless you need further customization for your exact use case. As is stated in [Terms & Conditions for the license](/en/dokumentation/villkor/) we recommend that a lawyer should go over the the License if the publisher of the API wants to be completely sure that the License reflect their exact conditions.

##3. Use the License
Take the customized License from the previous step and add it to your API documentation. Also require all users of the API to approve the License. It is recommended that the License is clearly marked with a version and made [reproducible](/en/dokumentation/rattsligaval/#aterskapa) by using a public version control system (i.e. [GitHub](https://github.com)). Do not forget to always [refer to the original license](/en/dokumentation/villkor/#hanvisning).

##4. Let us know that you are using the License
Send a mail to [info@apilicens.se](mailto:info@apilicens.se) if you are using the License and we would be happy to list your project on this site.

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Get Started with the License</h3>
<ol>	
	<li><a href="#1">Is this the right License?</a></li>
	<li><a href="#2">Customize the License</a></li>
	<li><a href="#3">Use the License</a></li>
	<li><a href="#4">Let us know that you are using the License</a></li>
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