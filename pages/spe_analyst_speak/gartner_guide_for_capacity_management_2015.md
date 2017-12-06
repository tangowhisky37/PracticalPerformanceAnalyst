---
layout: pagelayout
title: Gartner Guide For Capacity Management - 2015
---

### Introduction 

Before we dive into the Gartner Guide for Capacity Management tools let’s look at what Capacity Management means and the value it provides the IT organization within an enterprise.

According to [Wikipedia](https://en.wikipedia.org/wiki/Capacity_management) - “Capacity management is a process used to manage information technology (IT). Its primary goal is to ensure that IT resources are right-sized to meet current and future business requirements in a cost-effective manner. One common interpretation of capacity management is described in the ITIL framework. ITIL version 3 views capacity management as comprising three sub-processes: business capacity management, service capacity management, and component capacity management (known as resource capacity management in ITIL version 2).”

According to the [ITIL library](http://www.itlibrary.org/index.php?page=Capacity_Management) Capacity Management is defined as follows, “Capacity Management is the discipline that ensures IT infrastructure is provided at the right time in the right volume at the right price, and ensuring that IT is used in the most efficient manner. This involves input from many areas of the business to identify what services are (or will be) required, what IT infrastructure is required to support these services, what level of Contingency will be needed, and what the cost of this infrastructure will be.”

We quite agree with the ITIL Library definition of Capacity Management since it tends to spell out clearly the need to deliver the relevant IT resources (compute, network, storage, etc.) at the right amounts, at the right price and the right point in time. The ITIL Library goes a step further and talks about Capacity Management as a process being made up three sub-processes:

* Business capacity management (BCM) – Focus on Capacity Management from a Business impact and outcome standpoint.
* Service capacity management (SCM) – Focus on Capacity Management from a Service standpoint where views/outcomes/forecasts are provided for the entire Service as a whole.
* Resource capacity management (RCM) – Focus on Capacity Management as a Service from a Resource standpoint. This would ideally focus on the physical and virtual elements of the various systems (compute, network, storage, etc.) rather than a Business or a Service Capacity Management view.

You can learn more about the Capacity Management process and how it fits within the overall SPE (Systems Performance Engineering) process framework at the SPE 101 section here at Practical Performance Analyst.

### Common Industry Challenges

Our experience managing Performance & Capacity at organizations worldwide has given us an understanding of some of the challenges customer’s large and small face when managing IT capacity across their environments. Capacity Management traditionally has been one of the areas where IT organizations have had the least amount of maturity from an SPE (Systems Performance Engineering) standpoint. IT organizations within enterprises tend to have more maturity in the Performance Testing, APM (Application Performance Monitoring) and possibly NPM (Network Performance Monitoring) space because those are the areas which have larger visibility from a business standpoint and in most cases require smaller investments of time, resources and money to setup and maintain.

There are many reasons why Capacity Management has been ignored and relegated to the backburner and it’s impossible to summarize all of them within this document. However within this section we’ll look at some of the most common reasons why Capacity Management has traditionally been ignored and later in this article look at what potentially could organization do to address that gap.

* Capability required to define a mature capacity planning process – Capacity Planning or Capacity Management whatever you want to call it is a complex IT process which fits within the larger ITL process framework and requires significant investment (people, process, tools, etc.) within across the IT organization from an implementation/automation standpoint. Capacity Management is not seen as a mandatory function for an IT organization to have as a result many IT organizations have either very poorly defined processes or no processes at all. Combine that with the move to virtualization, cloud computing, consumptions of SaaS applications by business, outsourced management of applications and infrastructure, etc. and it’s not difficult to see what business and IT organizations have Capacity Management low down on their list of priorities. Let’s also take a look at the lack of Capacity Management capability within IT organizations from three different dimensions i.e. People, Process and Tools.
  * People – Capacity Management from a Business or Service Management standpoint requires strong technical capability combined with a good understanding of the basics of statistical modelling and in some cases analytical modelling. Finding such capability within IT teams has traditionally been challenging. Tools that perform such modelling, forecasting do help but still require capability technical engineers to put together the relevant modelling and forecasting techniques.
  * Process – SPE (Systems Performance Engineering) as a process across the Systems Delivery Lifecycle is pretty much missing in most organizations and it’s no surprise that Capacity Management is right at the bottom of the list within the SPE process framework. With the advent of the cloud and the digital age where business expects short delivery cycles for applications with quicker iterations the need for Capacity Management has pretty much gone out of the door. Businesses are relying more on their cloud partners to manage the capacity so that they can stay focused on building the applications and generating the revenue.
  * Tools – Costs and complexity of tools add to the woes. IT organizations today are mostly outsourced with vendors needing to support and manage IT infrastructure across the board. Vendors are mostly un-willing to invest in new tools or capability to automate capacity management and prefer managing capacity through use of outdated and complicated excel sheets with embedded unmanageable macros.
* Complexity of applications – Applications are getting complex all the time. The advent of the digital age combined with Cloud computing and SaaS based applications means that it’s very rare that any application sits within one single location and is owned by one single organization. The distributed nature of these applications combined with the lack of visibility across the various application components makes it challenging to obtain a view of performance and capacity across the entire Application Component Chain.
* Complexity of managing Hybrid Private / Cloud Environment – Most customers todays have migrated to using a combination of Private / Public cloud infrastructure. Vendor tools in some cases are playing catch-up. The cost of visibility across distributed infrastructure is higher with the need for more expensive and complex tools. The good old complex spread sheets that most organizations still use to manage capacity across the IT environments do not scale so well with hybrid environments.
* Complexity of deploying and managing Capacity Management tools – Capacity Management tools in most cases require dedicated capability within the IT team to deploy and run. With most IT organizations having outsourced the management of IT infrastructure vendors are unwilling to pick up the tabs for such expensive tools and fall back to either poor or no automated process for Capacity Management. The enterprise tools that provide good visibility are costly to procure/maintain and require dedicated capability within the IT organization which most customers are un-willing to pay. The advent of cloud computing has in some ways reduced the need for investment in Capacity Management since business would rather pay for additional IT infrastructure as required from the cloud vendor rather than pay for dedicated IT capability and tools within the organization to provide a view of the infrastructure they own.

### Considerations for purposes of tool assessment

Gartner’s market definition for Capacity Management includes the following perspectives –

* Capacity Management tools provide the capability to aggregate data from multiple sources while providing a view of the system performance through dashboards and reports
* Capacity Management tools provide capability for forecasting and trending of resource consumption across the various systems and tiers based on the data that it has collected from various systems
* The more advanced Capacity Management tools provide a view of performance optimizations, performance constraining factors including rule based automation to make changes to the infrastructure based on defined scenarios
* The more advanced tools provide integrations with a variety of domain specific tools including depth of analysis, ability to perform what-if analysis and integration with other OLAP and Business Reporting tools.

### Featured Players

The Gartner Guide for Capacity Management is not a Magic Quadrant and does not categorize players into the four different quadrants like the other Magic Quadrant reports do. This report rather reviews the leading players within the Capacity Management space and provides a point of view on the maturity of the product offering including the market segment the vendor focuses on from a Capacity Management standpoint. The list of players featured in the Gartner Guide for Capacity Management includes –

* ASG or Allen Systems Group 
  * URL - <a href="https://www.asg.com/" target="_blank">https://www.asg.com/</a>
  * Product - PerfMan
* BMC Software 
  * URL - <a href="http://www.bmc.com" target="_blank">http://www.bmc.com</a>
  * Product - Truesight Capacity Optimization
* Computer Associates (CA) 
  * URL - <a href="http://www.ca.com" target="_blank">ca.com</a>
  * Product - CA Capacity Management
* Cirba 
  * URL - <a href="http://www.cirba.com" target="_blank">http://www.cirba.com</a>
* Dell 
  * URL - <a href="http://www.dell.com" target="_blank">http://www.dell.com</a>
  * Product - Foglight for Virtualization
* IBM 
  * URL - <a href="http://www.ibm.com" target="_blank">http://www.ibm.com</a>
  * Product - 
    * SmartCloud monitoring
    * SmartCloud APM
    * Tivoli Netcool Performance Manager
    * IBM SmartCloud Virtual Storage Center
* Metron 
  * URL - <a href="http://www.metric-athene.com" target="_blank">http://www.metric-athene.com</a>
  * Product - Athene
* NetIQ 
  * URL - <a href="http://www.netiq.com" target="_blank">http://www.netiq.com</a>
  * Product - Platespin Recon
* Solarwinds 
  * URL - <a href="http://www.solarwinds.com" target="_blank">http://www.solarwinds.com</a>
  * Product - Solarwinds Virtualization Manager
* Sumerian 
  * URL - <a href="http://www.sumerian.com" target="_blank">http://www.sumerian.com</a>
  * Product - Sumerian Capacity Planner
* Teamquest 
  * URL - http://www.teamquest.com
  * Product  
    * Analyzer for Performance Analysis
    * Predictor for Capacity Planning
    * Surveyor for dynamic and automated analytics + reporting
    * CMIS
* Virtual Instruments 
  * URL - <a href="http://www.virtualinstruments.com" target="_blank">http://www.virtualinstruments.com</a>
  * Product - VirtualWisdom
* VMTurbo 
  * URL - <a href="http://www.vmturbo.com" target="_blank">http://www.vmturbo.com</a>
  * Product - VMTurbo Operations Manager
* VMware 
  * URL - <a href="http://www.vmware.com" target="_blank">http://www.vmware.com</a>
  * Product - vRealize

### Summary 

The Capacity Management market is nowhere as big as the APM (Application Performance Monitoring), Performance Testing or NPM (Network Performance Monitoring) market. Also the drive to cloud computing, outsourcing of applications and infrastructure along with increased consumption of SaaS based applications means that IT organizations are going to invest less in building Capacity Management capability within the organizations and rely more on their partners and vendors to perform Capacity Management.

The enterprise tooling capability required combined with the maturity required to build and deliver Capacity Management make it an expensive process which most IT organizations are going to un-willing to spend on. However with the increase in use of ITOA (IT Operational Analytics) tools like Splunk, etc. there is a very high possibility that these vendors will start moving into the Capacity Management space by providing plugins or extensions that offer Capacity Management capability. Every ITOA (IT Operational Analytics) vendor is trying to grow their partner and plugin ecosystem and Capacity Management along with forecasting is potentially something we should expect to see available at some point in the near future.

Overall while Capacity Management is an important activity across the Systems Delivery Life cycle we forecast that status quo will continue. Business and IT organizations will continue to push Capacity Management onto their partners and vendors expecting them to take the onus of managing capacity across their IT infrastructure reducing the need to invest in building Capacity Management capability within the IT organization.
