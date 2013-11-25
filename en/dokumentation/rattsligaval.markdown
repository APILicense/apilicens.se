---
layout: post
lang: en
title:  "Legal Options"
date:   2013-11-24 6:42:00
---
A publisher of an API needs to consider all the laws that apply. This is a presentation of the laws that are relevant for an API, and the choices needed to be made based on these laws - hoices that in turn will impact the content of the [License](/en/dokumentation/licens). Depending on the choices the company makes the License will contain alternative texts, making the License flexible for many different use cases.

A short version of all available options can be found in the [Quick Choices](/en/dokumentation/vagval/).

##<a id="immaterialla">Intellectual Property Rights</a>

###<a id="upphov">Copyright Protection</a>
The Swedish Copyright in Literary and Artistic Works Act (SFS 1960:729) grants a person who has created a literary or artistic work the exclusive right to produce new copies of the work and to make it available to the general public, in all cases other than for purely private use.

Literary or artistic works can include a text, photograph, computer program or musical work, provided the text, photograph, computer program or musical work is sufficiently original.

As in any other case where a company wishes to distribute material which may be copyright-protected, the provider of an API must therefore check whether the API returns any material to which a party other than the provider of the API has copyright, or to which the API provider itself has copyright and wishes to impose limitations on the use of. 

Therefore, a company that provides an API should avoid displaying images, software code and other works in an API if there is uncertainty as to whether the copyright holder’s approval has been obtained to distributing the work in this way.

Occasionally, the right to use a copyright-protected work is subject to conditions, such as an image provided under a licence which states that the copyright holder must be mentioned when the image is copied or distributed. In order to comply with such conditions, an API provider should give the users (i.e. the developers who are granted access to the API) the information they need to prevent them from violating the copyright to any work, by communicating the terms and conditions governing the works which are provided via the API. 

Since these terms and conditions will vary from case to case, it is not possible to insert this information in the licence wording produced within the scope of the project, but the licence wording has been provided with scope for the API provider to describe any terms and conditions governing copyright-protected material.

In cases where the users themselves can generate information for the API, the API provider should make it clear that the user him/herself is responsible for ensuring that he or she is entitled to distribute any copyright-protected works, see [the description of warranties](/en/dokumentation/affarsval). 

###<a id="varumarke">Trademark Protection</a>
The Swedish Trademarks Act (SFS 2010:1877) grants a person who has registered or established on the market a trademark the exclusive right to use the trademark in business activities. 

Examples of trademark-protected material include logos, trade names and symbols, provided they constitute a unique trademark.

As in the case of copyright-protected material, the provider of an API is not entitled to permit its users to use a trademark which does not belong to the API provider. Therefore, a company which provides an API should refrain from including trademark-protected marks in an API if there is uncertainty as to whether the holder’s approval has been obtained to permitting third parties to use the trademark. 

As in the case of copyright-protected material, if the API provider has obtained the right to permit its users to use a third-party trademark, the API provider should inform its users of any terms or conditions governing the use of the trademark. 

It may also be the case that the API provider wishes to require the user to make reference to the provider’s own trademark or company name when the user publishes information to which it gained access via the API. 

Some API providers may also wish to acquire the right themselves to refer to the user’s trademark or company name to advertise who uses the API. The use of trademarks in these situations is addressed in section 5.4 below.

####Options in the License
Will the API disclose material subject to intellectual property protection, such as material covered by copyright or trademark protection?

* Yes: retain [section 2.2 of the License](/en/dokumentation/licens#2.2) and insert desired information.
* No: Delete [section 2.2 of the License](/en/dokumentation/licens#2.2)

##<a id="pul">Personal Data Protection</a>

### Background
The Swedish Personal Data Act (SFS 1998:204) (PUL) sets out the conditions for automated processing of personal data in activities which are not of a purely private nature. 

“Personal data” is defined in PUL as “all kinds of information that directly or indirectly may be referable to a natural person who is alive”, which may include:

* A natural person's name
* A natural person’s email address
* An IP number which can be linked to a natural person 
* A username in a social network.

“Processing” means essentially any measure taken with respect to personal data, including collection, recording, organisation, storage, adaptation, alteration, use, disclosure by transmission, dissemination, compilation, blocking, or deletion. 

The provisions of PUL are aimed at the controller of personal data, i.e. the body which, either alone or together with other parties, decides the purpose and means of processing personal data. PUL lists a number of requirements which are imposed on the controller of personal data, including: 

* requirement for certain information for registered persons;
* requirement to take appropriate technical and organisational measures to protect the personal data being processed;
* requirement that the controller of personal data may not transfer personal data to a third party country (i.e. a country outside the EU/EEA) without legal grounds to do so.

###<a id="inhamtande">Obtaining Personal Data</a>
Many API providers require that users register certain information about themselves (such as their name and email address) in order to gain access to the API. The API provider is to be regarded as the controller of personal data in respect of personal data collected in this manner and, as a result, must comply with PUL’s requirements relating to a controller of personal data. 

Some of these requirements fall outside the scope of the project, but to give an idea of what information a controller of personal data should provide to registered persons (i.e. to users who have registered their information in order to gain access to an API), the licence contains a reference to a personal data management policy. The project recommends that an API provider provide, at a minimum, the information set out in the Personal Data Processing Policy template. 

####Options in the License
Will the API user need to register certain personal data (e.g. their email address or name) in order to gain access to the API?

* Yes: Retain [section 3.1 of the License](/en/dokumentation/licens#3.1).
* No: Delete [section 3.1 of the License](/en/dokumentation/licens#3.1)

###<a id="utlamning">Disclosure of Personal Data</a>
When a company wishes to disclose information containing personal data through an API, the assumption is generally that the company is the controller of personal data according to PUL, and that the disclosure of the data is to be regarded as personal data processing.

PUL states that there must be a legal basis for every act of processing (e.g. disclosure to an API user), which can either consist of the controller of personal data having obtained the registered individual’s consent to the processing, or the processing being necessary to enable performance of an agreement with the registered person, to enable the controller of personal data to perform a legal obligation or suchlike. (see section 10 of PUL).

Therefore, when an API is about to be launched, the provider must, as an initial step, check whether the information which is to be disclosed contains any personal data. If so, the provider must check that it has a legal basis for disclosing the information to the API users, for example by having obtained the consent of the registered users to doing so.

Since API users who receive the personal data will, in turn, become controllers of personal data in respect of their processing of the data, the project recommends that the API provider inform the users that they are responsible for ensuring that their own processing of personal data takes place in accordance with PUL. 

In cases where users themselves can generate information for an API, the API provider should make it clear that the user him/herself is responsible for ensuring that he or she is entitled to distribute any personal data made available by the user in the API, see [the description of warranties](/en/dokumentation/affarsval). 

###Options in the License
Will the API disclose personal data?

* Yes: Retain [section 3.2 of the License](/en/dokumentation/licens#3.2).
* No: Delete [section 3.2 of the License](/en/dokumentation/licens#3.2)

##<a id="aterskapa">Requirement that the Licence be capable of being reproduced</a>
The Swedish Electronic Commerce and Other Information Society Services Act (SFS 2002:562) (the “E-Commerce Act”) contains a number of requirements as to the information a provider of “information society services” is permitted to disclose to its users. 

As is clear from the limitations which have been imposed on the project, we have concluded that most of these information requirements need not be satisfied in the wording of the licence itself, but, rather, can be stated elsewhere on the website on which an API is being provided. 

However, section 13 of the E-Commerce Act contains a requirement that “contractual terms and conditions must be made available to recipients in a way that allows them to store and reproduce them”.

Therefore, the project recommends that API providers provide their licence wording in a public version management system (e.g. [GitHub](https://github.com)), as a PDF or in an equivalent format which makes it possible for API users to store and reproduce it. 

In cases where an API provider has modified a provision in its licence wording, the company should publish a new version of the licence in a format which can be stored and reproduced by the users. As regards communicating changes to the licence wording to users, see also section 5.6 below.

###Implication for the License
See [section 7.2 of the License](/en/dokumentation/licens#7.2).


{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Legal Options</h3>
<ul>
	<li><a href="#immaterialla">Intellectual Property Rights</a></li>
	<li><a href="#upphov">Copyright Protection</a></li>
	<li><a href="#varumarke">Trademark Protection</a></li>
	<li><a href="#pul">Personal Data Protection</a></li>
	<li><a href="#inhamtande">Obtaining Personal Data</a></li>
	<li><a href="#utlamning">Disclosure of Personal Data</a></li>
	<li><a href="#aterskapa">Requirement that the Licence be capable of being reproduced</a></li>	
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