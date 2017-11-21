---
layout: pagelayout
title: Howto Create A Performance Budget
---

The topics covered in this HowTo include:

* Introduction
* What are HowTo’s
* Why HowTo’s @ PPA
* Why We Wrote HowTo Create A Performance Budget
* What Are Non Functional Requirements
* So What Are Performance Budgets
* What Tiers Should Be Considered In Scope When Defining Performance Budgets
* How Does Performance Budgets Align With Non Functional Requirements
* How Important Are Performance Budgets
* Who Should Own, Design and Maintain Performance Budgets
* At What Point In The Development Life Cycle Should Performance Budgets Be Created
* Let’s Create A Performance Budget
* What Outcomes Should You Expect To Achieve With Performance Budgets
* Measuring and Tracking How Teams Are Tracking With Their Performance Budgets
* Caveats And What To Be Careful Of When Designing Performance Budgets
* Conclusion

### What Are HowTo’s

A HowTo is a document that does precisely what the name suggests i.e. It’s describes “HowTo” achieve a set of outcomes through illustration of all the steps involved. HowTo’s are generally structured and written without too much technical jargon in a straight forward manner without making too many assumptions of the depth of knowledge the reader. HowTo’s are meant to make for easy reading and are logical in the sequence of steps it recommends.

Any background knowledge to assimilate the information provided in the HowTo is generally highlighted at the start of the HowTo. HowTo’s are generally written for the professional who are clear of what they need to accomplish but have little or no knowledge of how to go about achieving those objectives. HowTo’s are meant to be exhaustive in nature and they are definitely not meant to offer the most efficient way of getting the job done. A HowTo should be seen as a kick starter that helps the user get up and running with a given task without having to master all the required fundamentals.

Why HowTo’s @ PPA: HowTo’s have been the mainstay of the Open Source and Free Software movement for decades. One of the reasons why Open Source and Free Software is so widely used today is simply because of the depth of documentation that exists and the maturity of the Open Source ecosystem which has delivered scalable, open and reliable software. HowTo’s like many other building blocks have helped the Open Source and Free Software movement grow immensely while eliminating the need to keep re-inventing the wheel. It’s only natural that we at Practical Performance Analyst adopt the best from the Open Source and Free Software movement. A lot of the work we do at Practical Performance Analyst borrows from the fundamentals of the Open Source movement and HowTo’s are definitely one of them.

As HowTo’s @ PPA grows and matures we will hopefully reduce the reinventing of the wheel which happens so very often at organizations, projects and programs when it comes to the science of building/delivering systems that scale.

### Why We Wrote, HowTo Create a Performance Budget

A long time ago, as part of a customer engagement I was tasked with creating a performance budget for a system that was in the process of being designed and built. I asked myself, “What is a Performance Budget” and the answers I got back was:

* A way of accounting for the work done by employees and its impact against the total estimated work
* Some sort of project management methodology mainly concerning finances
* Some sort of accounting mechanism used to track program finances

It soon turned out that I was completely wrong and none of my so called definitions were anywhere close to the real definition of “Creating A Performance Budget”. So I decided to dig around a bit more and learn the science of creating Non Functional Requirements including creating associated Performance Budgets. This HowTo is a culmination of all that effort and learning I’ve gained over the last 8 months. I share this with the hope that others do not have to re-invent the wheel again when it comes to defining Performance Budgets. We hope the content in this HowTo including all other future HowTo’s at Practical Performance Analyst helps you embed stronger Proactive Performance Management or Proactive SPE (Systems Performance Engineering) practices within your organization, program or project.

### What are Non-Functional Requirements (NFRs) 

Non Functional Requirements are a definition of those attributes of a system that provide an understanding of the various “ties” i.e. performance, scalability, reliability, availability, etc. Non Functional attributes for a given system ensure that in addition to meeting to functional goals as laid down by the business, the system is also able to process the submitted queries in a timely, efficient, reliable and secure manner.

Here’s how Wikipedia defines Non Functional Requirements:

“In systems engineering and requirements engineering, a non-functional requirement is a requirement that specifies criteria that can be used to judge the operation of a system, rather than specific behaviors. This should be contrasted with functional requirements that define specific behavior or functions. The plan for implementing functional requirements is detailed in the system design. The plan for implementing non-functional requirements is detailed in the system architecture.

Broadly, functional requirements define what a system is supposed to do and non-functional requirements define how a system is supposed to be. Functional requirements are usually in the form of “system shall do <requirement>”, an individual action of part of the system, perhaps explicitly in the sense of a mathematical function, a black box description input, output, process and control functional model or IPO Model. In contrast, non-functional requirements are in the form of “system shall be <requirement>”, an overall property of the system as a whole or of a particular aspect and not a specific function. The systems’ overall properties commonly mark the difference between whether the development project has succeeded or failed.

Non-functional requirements are often called qualities of a system. Other terms for non-functional requirements are “constraints”, “quality attributes”, “quality goals”, “quality of service requirements” and “non-behavioral requirements”.[1] Informally these are sometimes called the “ilities”, from attributes like stability and portability. Qualities, that is non-functional requirements, can be divided into two main categories:

* Execution qualities, such as security and usability, which are observable at run time.
* Evolution qualities, such as testability, maintainability, extensibility and scalability, which are embodied in the static structure of the software system.”

You can read more about Non Functional Requirements at the following [Wikipedia link](http://en.wikipedia.org/wiki/Non-functional_requirement).

### What are Non-Functional Requirements (NFRs)..continued:

NFRs are generally technical requirements that are not very verbalized by the client, but need to be addressed to ensure the system delivered scales to meet customer needs. They address the operation of the system versus the behavior of the system. Non-Functional requirements are sometimes referred to as the “ties”. Here’s some of the important ones that come to mind:

* Scalability
* Availability
* Security
* Usability
* Maintainability
* Reliability
* Performance
* Backup
* Disaster Recovery & Fault Tolerance

While the above list is not exhaustive, it does provide a list of the most common dimensions one would consider when considering putting together non-functional for a given system. Without a clear understanding of Non Functional Requirements for a given system, the best written and implemented functional requirements will more than likely fail. If functional and non-functional requirements were a car, think of the functional requirements as the exterior and interior of the car and the non-functional requirements as the metrics that define how long does it take the engine to get you from 0-100 Km/Hr when you hit the accelerator including how long does it take your car to come to a stop when you are at 100 Km/Hr and you’ve just slammed on the brakes.

An example of a Non Functional Requirement is:

* Utilization of the application and database tiers should be <= 75% for peak workload during normal operations including Disaster Recovery conditions.
* 95th Percentile Response times for the login transaction should be <= 5s for peak workload during normal operations

Non Functional Requirements are a critical part of the solution design. Lack of understanding of Non Functional Requirements are some of the reasons why systems deliver poor end user experiences.

### So What Are Performance Budgets

Performance Budgets are a translation of the system Non Functional Requirements into performance objectives for each of the relevant system components. Lets review a few examples:

* End to End response time for a given business critical transaction is 5s.The Performance Budget for the web server is 0.2s, the application server is 2.8s and the database is 2s.
* End to End response time for a workflow is 10mins. The Performance Budget for the validate user input process running on the application server is 30s.

The Performance Budget examples illustrated above focus on response times for a given transaction however, Performance Budget can apply to any Non Functional attribute of a system across any of the components of the system i.e. from unit level code (written by a developer) to the performance of an entire container i.e. virtual machine or even physical host. Performance Budgets are applicable across various tiers of systems and across various system components.

### What Tiers Should Be Considered In Scope When Defining Performance Budgets

The value of splitting down the overall Non Functional Requirement into a Performance Budget for a given tier depends on the criticality of the transaction and the weight of the business transaction when it comes to processing at that given tier. For e.g. The business transactions in the above examples all traverse Firewalls, load balancers, SSL Accelerators, Core Switches, Data Center Switches, Web Server, Application Servers, Databases and then Messaging servers before going back out in to the world to other systems.

While the transaction does traverse through a lot of systems to get where it needs to get to you might not want to consider all those components for purposes of defining your Performance Budget simply because a lot of those tiers from experience (including your gut feeling) contribute almost nothing to the overall performance overhead i.e. it is well known that traversing the following network components Firewalls, load balancers, SSL Accelerators, Core Switches, Data Center Switches takes a few milliseconds on a local network and spending time optimizing these appliances to shave off additional microseconds isn’t going to give your great bang for your buck.

So use caution when setting Performance Budgets for the relevant tiers of your system. If in doubt speak to your Performance Engineering SME’s, your Application Architects, your System/Infrastructure architects, your Network Architects, your Performance Testing Leads, etc. to work out what are the tiers of importance and where across the entire delivery chain are you most likely to be encountering performance issues. As you gain experience designing Non Functional Requirements including Performance budgets this challenge will become a lot easier.

### How does a Performance Budget align with Non-Functional Requirements

Non Functional Requirements as we’ve discussed above determine the overall Non Functional attributes of the system End to End. Performance Budget in comparison are defined specifically for a given tier or set of tiers. Performance budgets localize the overall Non Functional Requirements and help translate the End to End Performance Requirements into simple and achievable tier wise performance targets which developments, administrators and designers can focus on delivering.

Performance Budgets are also intended to help measure the current and/or estimated future state of several Non Functional Requirements. For example let’s look at the following aspects of Non Functional Requirements:

* Scalability – Can we vertically or horizontally scale our system and meet the needs of the new requirements without much if any additional time, money, and effort?
* Reliability – Will modifications to the system or changes to the volume cause erratic behavior?
* Performance – If changes are made to the system, will we meet continue to meet our Service Level Agreements or technical expectations?
* Extendibility – Can we build upon the current system or do we need to implement something completely new?

In essence, a performance budget helps to answer questions about how current and future state modifications to hardware, software, code, etc. will impact the overall performance of a system or system process. Breaking down end to end Non Functional Requirements into Performance Budgets allows the Developer, Architect, Performance Tester, Performance Engineer, Capacity Planner, etc. understand the target for each of the relevant system tiers and how changes to the code/configuration/hardware will impact performance of the individual component.

Performance budgets are a means to measure how well an application can process data at relevant tiers e.g. what performance can one expect from an application server with regards to receiving, processing and transmitting data for a given transaction. Performance Budgets are broken down across tiers and are put in place to determine how fast information gets from point A to point B, from point B to point C, etc.   A performance budget can be designed for a closed or integrated application. An example of a closed application would be an n-tier Java EE application that sends and receives data from a database. In this case, you may want to measure how fast data moves from the user interface to the business logic layer, from the business logic to the data model layer, etc. On the other hand, an example of an integrated application could be an Enterprise SAP process flow that:

* Uses web services to submit customer orders
* Send requests for materials to third party vendors
* Provides on demand status to the customer
* Builds and ships goods to the customer
* Sends a bill and receives payment from the customer.

Performance Budgets simply put are translation of your Non Functional Requirements into tier wise targets that developers, systems administrators, architects, etc. can work towards when designing and building the relevant system components they are responsible for.

Performance Budgets metrics are based on one or more of the following dimensions:

* Current state performance metrics
* Estimated increases/deceases in volume or message size
* Estimated increases/decreases in processing power of hardware

This information can be easy to obtain if the IT Infrastructure, Architect, and Development Teams are maintaining and tracking these metrics closely or very difficult if the information is not being tracked inaccurately or not at all. Performance metrics tend to come from custom built or commercial performance monitoring tools.

### How important are Performance Budgets

Performance Budgets are very useful in setting targets for each of the relevant teams and guiding them through the objectives they need to be working towards from a Non Functional standpoint.

Performance Budgets help provide technical stakeholders with an initial picture of where performance issues may occur. They guide interested parties in scoping out potential performance problem areas by reviewing metrics such as response time and noting how the timings between individual components that have a potential to impact the overall process.

Performance Budgets provide Development Teams with performance goals for a newly created or modified aspect of a given process, and allows technical leadership teams to provide a technical expectation of how fast a process should occur and hold accountable parties to the standard. Performance Budgets together with Non Functional Requirements either reinforce or help in establishing Service Level Agreements and Operation Level Agreements (SLAs and OLAs) for a given process which help business teams and other non-technical stakeholders assess how quickly they can deliver goods and services.

Non Functional Requirements including Performance Budgets are key input into your Performance Testing approach where you would validate the scalability, performance and reliability of your system. With a clear view of Performance Budgets identifying and addressing performance issues becomes a lot more simpler due to the fact that the various tier leads now have clear visibility (and hopefully ownership as well) of the performance outcomes of their own tiers.

### Who should Design, Own, and Maintain Performance Budgets

The designer of performance budgets should be a person who understands the current/future state performance of the system/system process and can articulate this information in way to help developers, architects, and testers understand how the system should perform. The designer is a person who’s probably a technical resource such as a performance engineering specialist, an architect, or an infrastructure specialists who have a stake in the overall performance of the system. It is important that this resource understands the flow of the transaction across the system, is technically capable of mapping the relevant tiers and most importantly has the ability to work with all the tier design leads across the delivery chain to agree on the overall/tier wise performance budgets.

The designer will engage with business and technical stakeholders to fully understand system performance including how it should operate under normal and stressed circumstances. The owner of the performance budget is the person or team most concerned with the NFRs; ranging from the Architect, Infrastructure, to the Performance Team, or it could be a combination of all of the above. Ideally, the resource would be sitting within the Architecture team with visibility of the entire solution stack. Such a resource would also have visibility of the entire delivery chain given their role and would be able to influence design decisions including getting the relevant tier leads to buy into Performance Budgets for their relevant tiers.

At what point in the Development Lifecycle should Performance Budgets get created: There is no hard and fast rule here but generally we would recommend that Performance Budgets be created during the Architecture and design phase of the project. The optimal time to design Performance Budgets are generally after functional design completes and before technical design has completed. During this time both technical and functional requirements should have been determined and the expected modifications to both the hardware and software components should be known. Availability of historical data and/or estimates that support potential modifications or development of new processes to the system would make development of Non Functional Requirements including associated Performance Budgets a lot easier.

Performance Budgets along with design documents provide technical stakeholders with the relevant guidelines for designing/building/modifying applications, but also the required performance parameters that allow the process to meet or exceed both business and technical expectations.   These budgets aid in determining the impact of modifications to a system and what steps should to be taken to accommodate these changes.

### Let’s Create A Performance Budget

Performance Budgets can be used to measure key metrics the Performance Engineering or Performance Testing team are concerned with. Let’s look at an example to help illustrate the process we would follow to go about defining Performance Budget for a given set of tiers.

Application response times between portions of an application flow is a good example of a performance metric that will be of interest to both the business and technical stakeholders. Application Response Times are also “always” defined as part of the overall Non Functional Requirements for a given system. So it does make a lot of sense to translate the End to End Response Time Non Functional Requirement to a tier wise Performance Budget to help to design, development and build teams understand what performance specifications are they supposed to conform to.

![Process Flow]({{ "/assets/img/perf_budget.png" | absolute_url }})

The diagram above represents a simplified version of a performance budget. For purposes of this example the Performance Budget only concerns itself with response time. The response times could have been generated from log files, Application Performance Monitoring (APM) tools, a home grown solution, etc. A budget like the one above could be used as a starting point to help technical stakeholders understand current state performance and determine how modifications to either the software or the hardware may change portions of the response time. In addition, business stakeholders can get a clearer picture of what happens once the customer hits the submit button. In addition the above diagram helps business stakeholders develop SLA’s (Service Level Agreements) and OLAs (Operational Level Agreements) that both they and the technical stakeholders can be comfortable supporting.

What are the outcomes you wish to achieve with Performance Budgets: Following are the outcomes we would recommend you should be aiming to accomplish when expending energy determining Performance Budgets:

* Ensure alignment across the various application and infrastructure teams when it comes to an understanding of the End to End Non Functional Requirements
* Ensure understanding across the various application and infrastructure teams with regards to the relevant Non Functional Requirements that apply to their relevant systems/tiers
* Ensure buy in and ownership of the relevant Performance Budgets across the various application and infrastructure teams
* Ensure that the Architecture and Design for the system has taken into account the Non Functional Requirements and Performance Budgets that have been put in place.
* Ensure that all your stakeholders (Business and IT) have an understanding of the various Non Functional Requirements and Performance Budgets and have signed up to them.

There is a lot of merit in spending time working through your Performance Budgets and translating your End to End Non Functional Requirements into Performance Budgets for the relevant tiers. The pain you take initially during the design process will put you on a firm footing for the longer term.

### Measuring & Tracking How Teams Are Tracking With Their Performance Budgets

Defining Performance Budgets is one thing but measuring them and tracking them is another challenge altogether. In this section we will look at how one might go about measuring and tracking Performance Budgets across the various phases of the program.

* Build Phase: Using unit performance testing tools and scripts i.e. Junit, etc.
* System Testing Phase: Using browser based Page Analysis tools including Network sniffers like Wireshark (Ethereal).
* Integrated Performance Testing Phase: Using Performance Testing tools like Load Runner, NeoLoad, Webload, etc.
* In Production: Using data from RUM (Real User Monitoring Tools), Diagnostics/APM (Application Performance Management) tools, etc.

### Caveats and what to be careful of when designing Performance Budgets

Designing Performance Budgets is like walking a tight rope. On one hand you want to ensure that you are getting the most bang for your buck and are designing systems that are responsive but on the other hand you want to ensure that the architecture that is being put in place is able to deliver to the numbers you are signing up to. Most of the times tier leads sign up to aggressive Non Functional Requirements and Performance Budgets without understanding the implications until later on in the program.

It is absolutely essential that you work collaboratively with rest of the build and design team to delivery realistic and sensible Performance Budgets but at the same time you want to be absolutely sure that what you are signing up to deliver is practically feasible, especially if you have contractual obligations that are going to be tied to the delivery of the Performance Testing reports which will validate the ability of the system to meet the documented Non Functional Requirements including the tier wise Performance Budgets.

### Conclusion

Realistic Performance Budgets are a key to delivering systems that scale. But putting together Performance Budgets and translating Non Functional Requirements to Performance Budgets is just the first step. Working with the design, architecture, built and test teams on owning and implementing the Performance Budgets is the next big piece of the puzzle. Working collaboratively with all your teams across the program to design and build relevant Performance Budgets will put you in a good position to validating the performance of the system against the defined Non Functional Requirements and Performance Budgets once the system is available for Integrated Performance Testing.
