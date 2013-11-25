---
layout: post
lang: en
title:  "Commercial Options"
date:   2013-11-24 9:11:00
---
These are the Commercial options that are the foundation for [the License](/en/dokumentation/licens), i.e. factors that needs to be considered depending on the content of the API. The commercial choices are dependent on the strategic choices the company publishing the API makes, e.g. regarding pricing and how the data from the API may be used. Depending on the choices the company makes the License will contain alternative texts, making the License flexible for many different use cases.

A short version of all available options can be found in the [Quick Choices](/en/dokumentation/vagval/).

##<a id="tekniska">Technical Requirements and Limitations</a>
It may be important from a commercial perspective how the API users will be able to cache, store and copy the information obtained via the API.

Some information is very time-critical (such as financial or traffic-related data) which means that storage can risk creating a poor experience for the end user. Other information is rarely updated, which reduces the risk associated with locally-stored data. Local storage of the API's users can also reduce the strain on the systems on which the API is used. 

Some companies need to be able to prevent large portions of their data being copied, since otherwise the entire existence of the company may be at risk. However, a prohibition on storage may be viewed by the API’s users as an obstruction, for example where the developer already has a server infrastructure which it wants to use or where the information needs to be processed before being shown to final users. For other developers who develop services which are very similar to the structure of the API, direct use without the need to establish its own server infrastructure may be viewed in a positive light. 

If the API owner obstructs API users from storing data, this may also prevent the development of certain types of services (services which one could perhaps not even have conceived of developing from the outset), such as services where statistics are compiled and presented based on different types of real-time data. 

In light of these types of considerations, the API user should determine whether it wants to impose any limitations on the user's right to cache, store and copy information from the API, and, if so, whether the user should be responsible for updating stored data.

It is up to the individual API provider to determine precisely which technical limitations and possibilities should be offered to the user, but the project recommends that a provider provide the information set out in the Technical Documentation template. 

###Options in the License
Are there any technical limitations on how the user can use the API content, e.g. applicable caches, storage, copying and updates in respect of the API content?	

* Yes: Retain [section 4.1 of the License](/en/dokumentation/licens#4.1) and delete any limitation which is not relevant. 
* No: Delete [section 4.1 of the License](/en/dokumentation/licens#4.1).

##<a id="betalning">Payment for Access to the API</a>
An important issue for API providers is in what way the API should be profitable. In some cases, this may only involve increasing in the number of services which means that more customers or other interested parties can be reached on platforms and in connections which match their preferences. In other cases, the company may be the owner of information which is otherwise difficult or impossible to get hold of, and which the company wants to get paid for. In still other cases, a hybrid model may be applied where there is a “free level” and one or more “pay levels” (where the developer gains access to additional information or more calls per given amount of time).

In cases where the content of the API is either wholly or partly subject to a fee, the project recommends that the licence refer to a separate price list. 

###Options in the License
Do you want to charge a fee for the use of the API?

* Yes: Retain [section 5.2 of the License](/en/dokumentation/licens#5.2).
* No: Delete [section 5.2 of the License](/en/dokumentation/licens#5.2). 

##<a id="kommersiell">Commercial Use of Information from the API</a>
Making possible commercial use of an API is often something which makes it more attractive for the API users to develop services on the API, but in some cases an API provider would not want external developers to design services which profit from the provider’s information.

If an API provider wishes to limit the possibility to use information from the API for commercial purposes, it is important to establish clear limitations as to what is to be regarded as commercial use. For example, can users of the API develop a service which contains adverts? 

###Options in the License
Are there any limitations as regards the commercial use of information from the API? 	

* Yes: Retain one of the options in [section 5.3 of the License](/en/dokumentation/licens#5.3) *or* include a seperate limitation.
* No: Delete [section 5.3 of the License](/en/dokumentation/licens#5.3).

##<a id="hanvisning">Reference to Source</a>
Specifying where information from the API has been obtained, for example by using the API owner's logo, can (depending on the service) generate both positive and negative effects for the API owner. Many API owners choose to provide specific trademarks or guidelines for this situation, such as “Powered by XXX”. However, it may be unreasonable to require the API user to specify this information, for example if the service uses a large number of data sources that impose the same requirements, resulting in the entire service being flooded with source information. 

It is important to draft an API licence in a way that ensures that reasonable requirements are imposed in this respect. The licence should state clearly which requirements are imposed as regards referring to the source. This may typically involve the following: 

* No reference is permitted to be made (i.e. the data source must be completely anonymous).
* The name/logo/link to the data source must be displayed to the end user in a way that makes it clear which data sources are being used. 
* Each and every portion of the data which comes from the API must be labelled in such a way that the end user understands precisely where the relevant quantity of data comes from.

The user's obligation to refer to the data source should no longer apply when/if the user’s licence to use the API terminates (cf. section 8.4 of the licence wording). 

Certain providers of APIs may also wish to acquire the right to refer to the user's trademark or company name to advertise who uses the API.

###Options in the License
Will the API user be obligated to refer to the data source?

* Yes: Retain Option.1 i [section 2.3 of the License](/en/dokumentation/licens#2.3) and insert desired information. Delete Option 2. Also retain the highlighted wording in  [section 8.4 of the License](/en/dokumentation/licens#8.4).
* No:. Retain Option 2 in [section 2.3 of the License](/en/dokumentation/licens#2.3). Delete Option 1. Also delete the highlighted wording in [section 8.4 of the License](/en/dokumentation/licens#8.4).

As an API provider, do you want to have the right to refer to the API user’s trademark/company name?

* Yes: Retain [section 2.4 of the License](/en/dokumentation/licens#2.4).
* No: Delete [section 2.4 of the License](/en/dokumentation/licens#2.4).

##<a id="kvalitet">Quality and Accuracy</a>
###Reporting errors and omissions
For API providers who wish to maintain high quality and accuracy in data provided by the API, the project recommends that a specific channel of contact for reporting errors in data be provided, such as an email address to which the API’s users can report any errors or omissions in data obtained. However, this is of course only applicable if the user actually has the resources to read and follow up the reports made. 

####Options in the License
Will the API’s users have the opportunity to report errors or omissions in the information which has been obtained?	

* Yes: Retain [section 6.1 of the License](/en/dokumentation/licens#6.1) and unsert desired information.
* No: Delete [section 6.1 of the License](/en/dokumentation/licens#6.1).

###<a id="garantier">Warrenties</a>
A question that often comes up for API providers is who is responsible for the quality and accuracy of the API information. This is often a question of who can be held responsible if, for example, an API returns incorrect information which then has an adverse effect on the end user (i.e. the party using the API user’s services). 

The responsibility can partly apply to the information which the API provider has generated, and partly to the information which has been generated by the API's users, provided the API permits information to be written back to the API provider. 

It is a purely commercial issue whether the API provider should undertake responsibility for the information it has itself generated, and a decisive factor is often whether or not the API is provided in exchange for payment, since a user who pays for access to an API can be regarded as having reasonable grounds for having higher expectations as regards the quality of information than someone who gets the information for free.

However, the project recommends that providers be careful about promising too much, and that, if they provide any warranties at all as regards the quality, reliability, etc. of the API content, they should only promise SLA levels or provide warranties regarding accuracy, etc. which they are certain they can satisfy. 

As stated in [section 6.3 of the License](/en/dokumentation/licens#6.3), the project recommends that an API provider exclude liability for indirect loss, such as loss of profit, etc. because such loss is very difficult to predict and, consequently, to “budget for” . The API provider should also impose a monetary cap on its liability. 

In cases where the API’s users can generate information for the API, the licence should specify that the user is responsible for ensuring that he or she has the necessary rights to the information which the user makes available (in respect of e.g. copyright and trademarks), and that the user is otherwise entitled to distribute the information, for example by the user having a legal basis for distributing any personal data which is transferred. 

###Options in the License 
Will any warranties be provided as regards the quality and accuracy of the information?

* Yes: Retain Option 1 in [section 6.2 of the License](/en/dokumentation/licens#6.2) and insert desired information. Delete Option 2
* Nej: Retain Option 2 in [section 6.2 of the License](/en/dokumentation/licens#6.2). Delete Option 1.

Will the API user be able to generate information for the API?

* Yes: Retain [section 6.4 of the License](/en/dokumentation/licens#6.4). 
* No: Delete [section 6.4 of the License](/en/dokumentation/licens#6.4). 

##<a id="forandring">Handling Modifications to the API</a>
When managing open APIs, modifications must be handled in a structured manner, in terms of both technical modifications to the API itself and modifications to prices and the licence wording. 

The structure for handling modifications should be communicated to the API users to create realistic conditions for the way in which a developer will be able to use the API.

The conditions for handling modifications tend to vary between different API providers and require relatively detailed explanations, but the project recommends that a provider provide, at a minimum, the information set out in the Modifications Policy template. 

###Implications for the License
See [section 7.1 of the License](/en/dokumentation/licens#7.1).

##<a id="skada">Damage and Suspension</a>
An API provider may wish to limit the use of the API by specifying that the API is not permitted to be used to develop services which prejudice the API owner, for example where the service in question is contrary to the API owner’s values or runs counter to the API owner’s business. 

To ensure that this type of wording is understandable to the API users, it is important that it is made clear what is meant by the API provider’s values and what is to be regarded as damaging to the API provider’s business. 

###Options in the License
Do you want to limit the use of the API for purposes which risk damaging your business?

* Yes: Retain [section 5.4 of the License](/en/dokumentation/licens#5.4) and insert desired information.
* No: Delete [section 5.4 of the License](/en/dokumentation/licens#5.4)

##<a id="uppsagning">Termination</a>
In cases where a user has paid a fee to gain access to the API (for example, by means of a subscription), the API provider may wish to impose limitations on the user's right to terminate the agreement, by prescribing that they have to give a certain number of weeks’ notice of termination or by permitting the user to terminate his or her connection with immediate effect but, if so, requiring that he or she compensate the provider for the remaining term of the contract.  

###Options in the License
Will there be limitations on the user’s right to terminate the licence?

* Yes: Retain Option 1 in [section 8.3 of the License](/en/dokumentation/licens#8.3) and insert desired information. Delete Option 2.
* No: Retain Option 2 in [section 8.3 of the License](/en/dokumentation/licens#8.3) and insert desired information. Delete Option 1.

{% sidebar %}
{% include documentation_sidebar.markdown %}

<div class="well">
<h3>Commercial Options</h3>
<ul>
	<li><a href="#tekniska">Technical Requirements and Limitations</a></li>
	<li><a href="#betalning">Payment for Access to the API</a></li>
	<li><a href="#kommersiell">Commercial Use of Information from the API</a></li>
	<li><a href="#hanvisning">Reference to Source</a></li>
	<li><a href="#kvalitet">Quality and Accuracy</a></li>
	<li><a href="#forandring">Handling Modifications to the API</a></li>
	<li><a href="#skada">Damage and Suspension</a></li>
	<li><a href="#uppsagning">Termination</a></li>
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