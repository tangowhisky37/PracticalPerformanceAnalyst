---
layout: pagelayout
title: Gartner Guide For Performance Testing - 2015
---

### Introduction

To understand the scalability limitations of the systems you are developing or to identify potential bottlenecks across the system one of the most widely used approaches is to performance test the system. Performance Testing is also commonly known as -

  * Stress Testing
  * Stress Volume Testing
  * Load Testing

Each of the above terms actually, means something slightly different (in terms of the nature of workload injected into the system) however for purposes of this article we will treat all of them as one and the same thing and refer to Performance Testing also as Stress & Volume Testing (SVT). To be able to performance test an organization need to make an investment in performance testing tools including the capability required to use the tool to generate the workload and execute the required performance tests.

Performance Testing is an integral part of Performance Engineering and as an activity that is generally performed reactively at the end of the system development life cycle. The result of Performance Testing late in the system development life cycle results in potential show stoppers being found but at a significantly higher cost as compared to what it would cost to have used proactive Performance Test approaches to identify defects early on in the system development life cycle.

The different types of performance tests you would have come across include -

* Stress testing
* Break testing
* Volume testing
* Soak testing

In this article we will look at what the market landscape for Performance Testing tools looks like, we will review who some of the leading Performance Testing tool vendors are including looking at some of the challenges that are associated with regards to Performance Testing.

### Common Industry Challenges

Let's look at some of the most common challenges with regards to Performance Testing as experienced across the industry.

* **Lack of Non Functional Requirements** - One of the biggest challenges that organizations face is the poor understanding and documentation of Non Functional Requirements. This has traditionally been an issue with development of in-house applications however with the advent of the cloud, ecommerce and the digital paradigm things are beginning to change (hopefully for the better). We are now in a an age where a lot of organizations have their entire business models based on their web based applications and customers are beginning to expect to have access to their data / service from any device and from any location. This is starting to drive a fundamental shift in the way organizations look at defining their Non Functional Requirements. Hopefully we will see increasing maturing in this space over the coming years.
* **Lack of Production Sized Infrastructure** - The best possible outcomes for Performance Testing require production sized kit in the Performance Testing environment. This is also quite rare unless you are building a cloud based system where spinning up additional virtual machines for Performance Testing is a piece of cake. Performance Testing teams have traditionally used scaled down environments and resorted to devious means i.e. extrapolation of results, etc. to forecast what the application performance would look like for a Production Size kit.
* **Lack of adequate licenses for Performance Testing** -  Traditionally, Performance Testing tools have been really expensive and as a result most small and medium size enterprises have resorted to using Open Sources tool for purposes of Performance Testing. Some others due to affordability issues tend to use lower virtual user (concurrent user) licenses and increase the TPS (Transactional Throughput) to simulate what system performance might look like at higher volumes. This approach is highly dangerous and is known to provide misleading results.  * Lack of realistic and production like Workload models â€“ Making an investment in Industry Standard Performance Testing tools is one thing and begin able to draw up realistic, sensible Workload Models to performance test the applications is completely another issue altogether. Most organizations and IT teams lack the experience and understanding required to design and build realistic Workload models.
* **Lack of suitable APM and NPM tools** - Industry Standard Performance Testing tools are good to have, however to make good of your investment in the Performance Testing tools it's important to have the relevant APM/NPM tools to be able to dive into the system (application, middleware, database, etc.) to identify performance issues when things start going pear shaped during your Performance Test. Think of APM and NPM tools are your torch light that helps you get straight to the relevant areas of focus across the system.
* **Reactive approach to Performance Testing** - Performance Testing has traditionally been looked at as a reactive testing phase which is useful to identify show stoppers before go-live. This approach combined with the cost of addressing system, architectural defects late in the System Development Life Cycle suggest that a change in attitude might be tremendously useful. The Agile development movement and the DevOps movement have been trying to change this traditional view to testing and in a lot of cases seem to have successfully challenged the status quo.
* **Performance Testing = Performance Engineering** - Organizations might be good at Performance Testing but thinking that mature Performance Testing is good enough to help you stay competitive might not be a good idea. Organizational IT spend is getting slimmer by the year with increasing expectation for IT to outsource not just its services but also the infrastructure on which its applications are based. To ensure that the application and underlying systems continue to scale while the business grows it's important that IT organizations look at building capability across relevant parts of the Performance Engineering life cycle. The Performance Engineering lifecycle can be simply broken down into the following steps -
  * Non Functional Requirements definition
  * Workload Modelling
  * Performance Modelling
  * Capacity Planning
  * Performance Testing
  * Monitoring, APM & NPM
  * Capacity Management (Use feedback loop and go back to 1 above)

### What are the current Industry trends that impact Performance Testing

Here's some of the main trends that are impacting the industry and the uptake of Performance Testing tools worldwide -

* Increasing adoption of Cloud based solutions by business resulting in the need for Performance Testing tools to adapt to application protocols native to the web including challenges of scripting/execution in a shared environment.
* Increasing adoption of Agile and Devops as development practices that are trying to get development and production support teams to experience the pains of performance optimization early on in the development process.
* Increase in adoption of Micro Web Services which are driven by the need to stay modular and yet scalable.
* The emergence of the Digital Enterprise where organizations are now having to interact with the customers through online interfaces, present a simplified multi-channel strategy to the customer and manage the customer through various stages of the customer acquisition life cycle.
* The change in customer expectations where the customer is now expecting access to his/her data and services from any device and from any location.

The nature of changes in the last decade have revolutionized how Performance Testing and Performance Engineering as a service is conceived. The transition to Digital including the increased adoption of Devops/Agile development practices in many ways have increased the focus on Performance Testing capability and tooling within enterprises.

### What does the market look like from a Performance Testing tool standpoint -

The Performance Testing market has grown considerably over the years and we predict with the move to Digital combined with the increased adoption of Devops/Agile development practices the uptake of Performance Testing tools (OpenSource and Commercial) will only increase. Gartner estimates the current Performance Testing market to be around USD 690 Million in size and growing annually at the rate of 9.6% worldwide. Gartner estimates the overall size of the testing tools market at over USD 1.5 Billion in 2014.

### What are the dimensions to consider when selecting a Performance Testing tool

Investing in a Performance Testing tool requires considering various options, dimensions and parameters. Here's a view of some of the dimensions you should be thinking along when looking to make an investment decision on Performance Testing tools for your enterprise.

* Availability of expertise in the market on the given Performance Testing tool
* Ability of the vendor to provide local support
* Ability of the tool to integrate with the other APM (Application Performance Monitoring) and NPM (Network Performance Monitoring) solutions you use across the enterprise
* Ability of the tool to integrate with your Infrastructure monitoring solutions
* Support for a broad range of application protocols including the ones that are used across your organization e.g. SOAP, HTTP/S, SAP GUI, etc.
* Scalability limitations of the tool that do not impact your ability to generate workload for your applications
* Scripting environment that is flexible and makes it easy to develop, maintain scripts
* Ability to integrate with CI (Continuous Integration) tools like Jenkins, Bamboo, etc.
* Ability to schedule and run tests including the ability to share testing capability across the organization.

For additional details on Performance Testing tools including a detailed discussion on dimensions to consider when choosing a Performance Testing tool please visit the SPE HowTo section here at Practical Performance Analyst.

### Who are the Leading Commercial Players

Let's review some of the leading commercial players featured by Gartner in their Performance Testing landscape review for 2015.

* Automation Anywhere
* Blazemeter
* Borland
* CA Technologies (DevTest Solutions)
* HP 
  * Storm Runner
  * Load Runner
  * Performance Center
* IBM Rational
* Neotys Neoload
* Oracle Load Testing 
  * Oracle Real Application Testing
  * Oracle Application Replay Pack
* Parasoft Load Test
* Radview Webload
* SmartBear 
  * LoadComplete
  * LoadUI NG Pro
* SOASTA Cloud Test
* Telerik Test Studio
* TestPlan â€“ EggPlant Performance

### Who Are the Leading Open Source Players

Listed below are some of the leading Open Source players in the Performance Testing world.

* Jmeter
* The Grinder
* Locust
* Gatling
* Tsung

The Gartner Market Guide for Performance Testing tools also provides an in-depth comparison of the various Performance Testing tools in a matrix form. You will find this immensely helpful if you are looking to compare the above tools from a functionality and platform support standpoint.

### Summary 

Performance Testing tools and vendors have been evolving at a fast pace over the last few years in response to some of the industry disruptions we have discussed earlier in this article. We hope you have found this article useful in terms of boosting your understanding of the Performance Testing landscape including the options available to you from a tooling standpoint.

