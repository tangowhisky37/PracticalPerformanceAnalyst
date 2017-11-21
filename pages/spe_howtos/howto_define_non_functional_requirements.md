---
layout: pagelayout
title: Howto Define Non Functional Requirements
---

The topics covered in this HowTo are:

* What Are HowTo’s?
* Why HowTo’s @ PPA?
* Why We Wrote, HowTo Define Non Functional Requirements (NFRs)?.
* What are Non-Functional Requirements (NFRs)?
* What Are Performance Budgets?
* How does a Performance Budget align with Non-Functional Requirements?
* What Tiers or Components of a System Should Be Considered In Scope When Defining Non Functional Requirements?
* How important are Non Functional Requirements to the success of a program?
* What Information Do You Need To Design Non Functional Requirements?
* Who should Design, Own, and Maintain Non Functional Requirements?
* At what point in the Development Lifecycle should Non Functional Requirements get created
* What Process Should One Follow To Define Non Functional Requirements?
* What are the outcomes you wish to achieve with Non Functional Requirements?
* How To Get Your Teams To Buy Into Non Functional Requirements?
* Measuring & Tracking How Teams Are Tracking With Their Non Functional Requirements?
* Caveats and what to be careful of when designing Performance Budgets?
* How Do You Leverage Non Functional Requirements across other SPE (Systems Performance Engineering) activities through the Development Cycle e.g. NFR’s as input into Performance Testing?
* What Table Of Contents should I Be Considering When Writing a Non Functional Requirements Document?
* Let’s Create A Few Non Functional Requirements
* Conclusion

### Why We Wrote, HowTo Define Non Functional Requirements (NFRs)

Non Functional Requirements are to SPE (Systems Performance Engineering) what Functional Requirements are to the Development (Agile, Waterfalls, etc.) Cycle. Without a view of the agreed Non Functional Requirements it’s impossible to do any of the following tasks:

* Design a system to meet any “expected” performance, scalable or End User Experience targets
* Determine a suitable Performance Testing Approach
* Determine a suitable Capacity Management Approach
* Design an implementable APM (Application/System Performance Monitoring) Approach
* Determine a suitable Performance Modelling Approach, etc.

The reason for not being able to do any of the above is simple; without any understanding of your objectives and target state you can’t really work out what approach to take to get to the target state. It doesn’t make much sense trying to build a car if you don’t know who your target customer is, what are is the values your target customer has, what lifestyle your target customer lives and what roads/speeds he/she likes to drive on.

To know where you want to go, you first need to know where you currently are and once you’ve determined where you currently are you can map out an approach to take you to where you want to go. It’s easy, it’s simple, it’s common sense but rarely seen implemented on projects large and small.

### What are Non-Functional Requirements (NFRs)

Non Functional Requirements are a definition of those attributes of a system that provide an understanding of the various “ties” i.e. performance, scalability, reliability, availability, etc. Non Functional attributes for a given system ensure that in addition to meeting to functional goals as laid down by the business, the system is also able to process the submitted queries in a timely, efficient, reliable and secure manner.

Here’s how Wikipedia defines Non Functional Requirements:

_“In systems engineering and requirements engineering, a non-functional requirement is a requirement that specifies criteria that can be used to judge the operation of a system, rather than specific behaviors. This should be contrasted with functional requirements that define specific behavior or functions. The plan for implementing functional requirements is detailed in the system design. The plan for implementing non-functional requirements is detailed in the system architecture.

Broadly, functional requirements define what a system is supposed to do and non-functional requirements define how a system is supposed to be. Functional requirements are usually in the form of “system shall do <requirement>”, an individual action of part of the system, perhaps explicitly in the sense of a mathematical function, a black box description input, output, process and control functional model or IPO Model. In contrast, non-functional requirements are in the form of “system shall be <requirement>”, an overall property of the system as a whole or of a particular aspect and not a specific function. The systems’ overall properties commonly mark the difference between whether the development project has succeeded or failed.

Non-functional requirements are often called qualities of a system. Other terms for non-functional requirements are “constraints”, “quality attributes”, “quality goals”, “quality of service requirements” and “non-behavioral requirements”. Informally these are sometimes called the “ilities”, from attributes like stability and portability. Qualities, that is non-functional requirements, can be divided into two main categories:
* Execution qualities, such as security and usability, which are observable at run time.
* Evolution qualities, such as testability, maintainability, extensibility and scalability, which are embodied in the static structure of the software system.”_

You can read more about Non Functional Requirements at the following Wikipedia [link](http://en.wikipedia.org/wiki/Non-functional_requirement)

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

### What Are Performance Budgets

Performance Budgets are a translation of the system Non Functional Requirements into performance objectives for each of the relevant system components. Let’s review a few examples:

* End to End response time for a given business critical transaction is 5s.The Performance Budget for the web server is 0.2s, the application server is 2.8s and the database is 2s.
* End to End response time for a workflow is 10mins. The Performance Budget for the validate user input process running on the application server is 30s.

The Performance Budget examples illustrated above focus on response times for a given transaction however, Performance Budget can apply to any Non Functional attribute of a system across any of the components of the system i.e. from unit level code (written by a developer) to the performance of an entire container i.e. virtual machine or even physical host. Performance Budgets are applicable across various tiers of systems and across various system components.

### How does a Performance Budget align with Non-Functional Requirements

Non Functional Requirements as we’ve discussed above determine the overall Non Functional attributes of the system End to End. Performance Budget in comparison are defined specifically for a given tier or set of tiers. Performance budgets localize the overall Non Functional Requirements and help translate the End to End Performance Requirements into simple and achievable tier wise performance targets which developments, administrators and designers can focus on delivering.

Performance Budgets are also intended to help measure the current and/or estimated future state of several Non Functional Requirements. For example let’s look at the following aspects of Non Functional Requirements:

* **Scalability** – Can we vertically or horizontally scale our system and meet the needs of the new requirements without much if any additional time, money, and effort?
* **Reliability** – Will modifications to the system or changes to the volume cause erratic behavior?
* **Performance** – If changes are made to the system, will we meet continue to meet our Service Level Agreements or technical expectations?
* **Extendability** – Can we build upon the current system or do we need to implement something completely new?

In essence, a performance budget helps to answer questions about how current and future state modifications to hardware, software, code, etc. will impact the overall performance of a system or system process. Breaking down end to end Non Functional Requirements into Performance Budgets allows the Developer, Architect, Performance Tester, Performance Engineer, Capacity Planner, etc. understand the target for each of the relevant system tiers and how changes to the code/configuration/hardware will impact performance of the individual component.


Performance budgets are a means to measure how well an application can process data at relevant tiers e.g. what performance can one expect from an application server with regards to receiving, processing and transmitting data for a given transaction. Performance Budgets are broken down across tiers and are put in place to determine how fast information gets from point A to point B, from point B to point C, etc.   A performance budget can be designed for a closed or integrated application. An example of a closed application would be an n-tier Java EE application that sends and receives data from a database. In this case, you may want to measure how fast data moves from the user interface to the business logic layer, from the business logic to the data model layer, etc. 

On the other hand, an example of an integrated application could be an Enterprise SAP process flow that:

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

For more details on Performance Budgets and HowTo go about writing Performance Budgets please see the “HowTo Define Performance Budgets” at the HowTo section at Practical Performance Analyst.

### What Tiers or Components of a System Should Be Considered In Scope When Defining Non Functional Requirements

Non Functional Requirements cover all the relevant aspects of a system being designed. Let’s take for example a Core Banking system with the following tiers:

* Firewalls
* SSL Accelerators
* Load Balancers
* IDS (Intrusion Detection Systems) and IPS (Intrusion Prevention Systems)
* Web Servers
* Application Servers
* Messaging Systems
* Workflow Engines
* Databases
* Business Intelligence & Reporting Systems

On such a system to be able to design your Non Functional Requirements you first have to put together a view of what are the critical components that are:

* Part of the delivery chain (responsible for doing work and delivering content to the customer)
* Have customer or business SLA’s attached to them
* Are responsible for delivering a great End User Experience
* Have IT OLA’s (Operational Level Agreements) attached to them

There is no hard and fast rule that specifies which set of systems on a project should or shouldn’t be part of the overall Non Functional Requirements. The answer to that question is more context driven and depending on what the project is on the hook to deliver.

If your system is a business critical system responsible for delivering a great End User Experience while also meeting internal SLA’s (To business) and external SLA’s to fee paying customers, you better have Non Functional Requirements that span the entire length of the delivery chain under your control i.e. from the Firewalls right up to the Business Intelligence and reporting systems including all the other systems in the middle. For such a system you would –

* Have Response Time targets that would be in line or better that your competitors
* Have utilization targets (infrastructure, network, etc.) that would ensure you have room for growth including peaks/troughs during the day/month/week of operation
* Have scalability targets i.e. concurrency, throughput, etc. that are equal to or higher than your peak workload of customers/business users
* Have performance metrics that suggest your system is running optimally and consuming relevant system resources in an efficient manner
* Have End User Experience targets that measure and track overall End User Experience
* Have SLA’s and OLA’s that are based on the internal SLA’s (to business) and external customer facing SLA’s that business have signed up to

On the other hand if you are dealing with a no business critical system which is used by a handful of people within the organization for some reporting tasks which are used in-frequently, you would still design relevant Non Functional Requirements but take a more realistic approach on the outcomes delivered. The Non Functional Requirements in this case would be a lot more realistic and less onerous that the ones you designed for the core business critical systems.

As we’ve mentioned earlier, Non Functional Requirements are a critical part of the solution design. Lack of understanding of Non Functional Requirements are some of the reasons why systems deliver poor end user experiences. So make sure you have worked through the relevant parts of the system, identified those components that are part of the solution whose performance/scalability matters to internal/external customers and then determine what coverage of Non Functional Requirements is critical to the success of your initiative.

Performance like many other things in life is about obtaining a balance. It’s a balance between spend and risk acceptance. If the risk appetite is low, your investment will be higher but if the risk appetite is high then the expected spend would be a lot lower.

### How important are Non Functional Requirements to the success of a program

Non Functional Requires are what underpins the success of any system. Without a view of the agreed Non Functional Requirements it’s impossible to do any of the following tasks:

* Design a system to meet any “expected” performance, scalable or End User Experience targets
* Determine a suitable Performance Testing Approach
* Determine a suitable Capacity Management Approach
* Design an implementable APM (Application/System Performance Monitoring) Approach
* Determine a suitable Performance Modelling Approach, etc.

The reason for not being able to do any of the above is simple; without any understanding of your objectives and target state you can’t really work out what approach to take to get to the target state. To know where you want to go, you first need to know where you currently are and once you’ve determined where you currently are you can map out an approach to take you to where you want to go. It’s easy, it’s simple, it’s common sense but rarely seen implemented on projects large and small.

Non Functional Requirements should be seen as a core part of the systems design specifications. While the functional specifications help identify the nature of functionality the program is expected to deliver, the non-functional attributes help clarify all of those important non-functional attributes e.g. scalability, reliability, availability, etc. that the program is on the hook to deliver. Non Functional Specifications set specific targets the Architects, Designers, Developers, Testers, Engineers, etc. can work towards achieving. Without specifications you have no objectives, nothing that the team can work towards. Expect a big large bun fight when the system gets into performance test and some real nasty surprises when you end up with your business critical system in production.

### What Information Do You Need To Design Non Functional Requirements

To design relevant Non Functional Requirements here’s the list of questions you should be asking yourself, your business, your IT counterparts, your application designers, your architects, your developers, etc.

* What are the components of the system that are part of the overall delivery chain
* What components of the system part of the overall delivery chain are we in control of
* What Service Level Agreements are we on the hook to meet
* What Operational Level Agreements are we on the hook to meet
* What is the impact of the system not being available? Can this be quantified?
* What is the impact of the system performing poorly? Can this be quantified?
* Are there other 3rd party components that are part of the current solution or design that will impact our ability to meet our SLA’s and OLA’s
* How critical is the availability of the application in terms of use productivity to your internal and external customers

Understanding what Non Functional Requirements is mostly about understanding the criticality of the service or business process that your system is being designed to support. It’s about understanding what lengths does the project team need to go to ensure that the system being designed, built, engineered and delivered is able to stack up to those expectations.

### Who should Design, Own, and Maintain Non Functional Requirements

Non Functional Requirements should generally be owned and driven by a senior program resource who displays the following attributes:

* Has a view of the overall solution architecture
* Has a strong understanding of the customers’ business
* Has a strong understanding of the customers IT landscape
* Has a strong understanding of the customer values and business criticality of the process the system is being designed to support
* Have the ability to identify the relevant resources across business and IT who are able to provide him an understanding of the SLA’s and OLA’s the system would need to meet
* Has the ability to articulate Non Functional requirements in a very non-technical manner to business and IT.
* Has the ability to communicate with business and IT in a non-technical manner working through their SLA’s and OLA’s with the objective of interpreting the dimensions of Non Functional Requirements that would be applicable
* Has the ability to take those high level Non Functional Requirements and translate them into detailed technical Non Functional Requirements which can be assigned to the relevant application and infrastructure teams
* Has the ability to take those high level Non Functional Requirements and translate them into tier wise performance objectives
* Has the ability to work closely with the Performance Testing, Diagnostics & Optimization leads to ensure that the results of the tests are in line with the overall Non Functional Requirements that have been documented and agreed to with business / IT.

### At what point in the Development Lifecycle should Non Functional Requirements get created

Non Functional Requirements are generally best written at the point where the design of the system is coming together. This is a point where the program and project leads have relevant context with regards to the overall solution architecture, overall technical architecture and also have a good understanding of the business process the customer intends to support using the system being delivered.

Given where you are with your project it’s highly possible that you won’t be 100% accurate on all fronts and you might have to leverage benchmarks/standards from other organizations (your customers’ competitors) to put together all the relevant Non Functional Requirements. It always helps to see what your customers competitors are doing and work through how better you can do it without having to burn a hole in your customers pocket i.e. While what we’ve mentioned above mostly applies to systems that are being developed from scratch there’s no reason why you couldn’t use the same rationale for projects where you are enhancing existing system functionality or are responsible for remediating existing systems.

The advantage of designing your Non Functional Requirements up-front is that you have the opportunity to work closely with business and IT to document the relevant technical specifications your system would need to meet to enable them meet their SLA’s and OLA’s. The other big advantage of doing this upfront is having the opportunity to work closely with your colleagues across the design, development and test teams to take ownership of the relevant application components and tiers wise Non Functional Requirements.


Whatever phase of the development cycle you are in, having an agreement on the expected outcomes i.e. the applicable Non Functional Requirements, how they will be measured, what the accepted tolerances are and what specifically the targets are they expected to meet, ensures that you have given each of the teams an opportunity to design/build/optimize relevant system components that hopefully when integrated work as expected towards delivering the expected End User Experiences meeting the relevant SLA’s/OLA’s.

### What Process Should One Follow To Define Non Functional Requirements

While there is no hard and fast process to document Non Functional Requirements, here’s what we recommend:

* Map out your business and IT stake holders
* Understand the appetite for risk on the program
* Understand the business processes that the system being designed is going to support
* Understand the existing system landscape and solution architecture
* Understand the existing SLA’s and OLA’s the system being designed will have to meet
* Work with business and IT to identify relevant dimensions of Non Functional Requirements that would be applicable to your project i.e. usability, reliability, availability, performance, scalability, etc.
* Work with business and IT on translating the SLA’s and OLA’s to end to end Non Functional Requirements for each of the various dimensions (mentioned above)
* Work with your project stream leads to translate the overall end to end Non Functional Requirements to tier wise Non Functional Requirements
* Work with business, IT and your stream leads to get a buy in on the overall Non Functional Requirements and your tier wise Non Functional Requirements
* Work with your Performance Engineering leads to measure, validate and track each of the Non Functional Requirements through the course of the project.

This process isn’t etched in stone. Feel free to take relevant parts of the process and apply it to your organization, project or program.

### What are the outcomes you wish to achieve with Non Functional Requirements

Following are the outcomes you would like to achieve with the Non Functional Requirements Gathering process:

* Ensure that relevant teams understand the relevant dimensions of Non Functional Requirements the project is responsible for delivering
* Ensure that everyone on the program has a view of the End to End Non Functional Requirements
* Ensure that relevant teams on the program understand the tier wise Non Functional Requirements they are on the hook for delivering
* Ensure that there is strong buy in from IT and business to the End to End Non Functional Requirements including the Tier wise Non Functional Requirements.
* Ensure that your performance engineering teams have the relevant tools, processes and capability to measure and track the relevant Non Functional Requirements through the course of the program

### How To Get Your Teams To Buy Into Non Functional Requirements

Getting your teams to buy into the Non Functional Requirements process is absolutely essential and one of the first steps you would take once you’ve nailed down the relevant Non Functional Requirements across the system. To get buy in you’re all the relevant teams across the program you need to ensure the following:

* Ensure your teams understand what Non Functional Requirements they are on the hook for delivering
* Ensure your teams understand what targets you’ve set for each of the Non Functional Requirements including acceptable tolerances
* Communicate to your teams the approach you’ve followed to design the End to End Non Functional Requirements and the Tier Wise Non Functional Requirements
* Communicate to your teams the SLA’s and OLA’s the application supports including the costs of business and IT not being able to meet the agreed SLA’s and OLA’s
* Ensure your teams accept that the documented Non Functional Requirements can be met with the overall solution architecture and system architecture that is being put in place

Without buy in from the various streams of your delivery team, your Non Functional Requirements is just a great looking document which will be of little use to anyone across the program.

### Measuring & Tracking How Teams Are Tracking With Their Non Functional Requirements

A wise man once said, to be able to fix something you need to be able to track it and to be able to track it you need to be able to measure it. To be able to measure how teams are progressing with delivery of the Non Functional Requirements you need to have a tracking mechanism setup. This could happen in many ways and here are some ideas that we propose:

* Setting up regular build checkpoints where the results of unit performance tests can be reviewed
* Regularly walking through the results of performance tests with rest of the teams and articulating where each of them are with regards to the Non Functional Requirements that they actually own
* Regularly reviewing the open defects across the system and providing everyone a view of how the various teams are progress with regards to the Non Functional Requirements they actually own.

The best way to measure progress of Non Functional Requirements is to get everyone together on a regular basis, review the defects and track performance of their teams with regards to the Non Functional Requirements they own. Keep in mind that you aren’t there to nail someone to the wall for the wrong they’ve done but rather to work with them constructively and help them meet their budgets so that in the end you are able to deliver a system that scales.

### Caveats and what to be careful of when designing Performance Budgets

Designing Performance Budgets requires that you understand the End to End Non Functional Requirements and also have an understanding of what would be a realistic breakdown of Non Functional Requirements across any of the tiers e.g. Performance targets split across the various tiers and what realistic numbers should look like. Try not to be too aggressive on the Non Functional Requirements you define. Work closely with the development teams to understand what’s an acceptable NFR based on industry standards combined with the SLA’s and OLA’s business has signed up to deliver. While it definitely pays not to be too aggressive when defining NFR’s, it also pays to understand how the systems works end to end so that you are able to define the relevant Performance budgets across relevant tiers of the system.

Define Performance Budgets working closely with your development and design team and keep them in the loop on how things are progressing. This will ensure that you get a lot more buy in from your teams and do not have to arm wrestle them into signing up to the documented Non Functional Requirements.

One of the other big challenges we’ve seen when designing and documenting Non Functional Requirements is the over zealousness of some of the design, architecture and build teams on accepting stringent Non Functional Requirements. Very often without visibility of the customization required and the complexity of the various interfacing systems teams agree to Non Functional Requirements which are quite impossible to deliver. One of the ways of eliminating this risk is to draw up the system (being developed) on a white boad and overlay the various relevant performance related NFR’s. Step through a tier wise break down of the Non Functional Requirements and relay past experiences with regards to the challenges you’ve faced meeting those requirements.

Customers are demanding and with technology deeply embedded in most aspects of our lives there is a huge surge in responsiveness of application interfaces. Be open the customers need which should reflect the market adoption but also be pragmatic of what the chosen architecture and system components can deliver.

### How Do You Leverage Non Functional Requirements across other SPE (Systems Performance Engineering) activities through the Development Cycle e.g. NFR’s as input into Performance Testing

Non Functional Requirements are the foundation of Performance Engineering activities across the SDLC. There are various ways Performance Engineers would choose to leverage Non Functional Requirements across the Life cycle. Here’s some examples:

* Non Functional Requirements during Performance Test to define your test outcomes
* Non Functional Requirements during Workload modelling to understand the workload characteristics of the system under test.
* Non Functional Requirements as the elements that underpin definitions of SLA’s and OLA.
* Non Functional Requirements as input in to designing your APM (Application Performance Monitoring) strategy
* Non Functional Requirements as an input into the Diagnostics & tuning approach

There are various ways Performance Engineers would leverage Non Functional Requirements across the delivery life cycle, most importantly being the definition of the overall Performance Testing Strategy. The emphasis on the End to End Performance Testing Strategy is simple because most systems are validated through a Performance Test to understand if it meets the documented Non Functional Requirements.

Non Functional Requirements are thus underpin the overall Performance Engineering approach highlighting the importance of getting it right the first time around.

### What Table Of Contents should I Be Considering When Writing a Non Functional Requirements Document

Here’s a summary of a Table Of Contents you might consider when designing your own Non Functions Requirements.

* Introduction
* Current & Historical Production Volumes
* User Concurrency Targets
* User Transaction Response Time Targets
* Infrastructure Performance Metrics and SLA’s
* Application Performance Metrics & SLA’s.
* End to End Performance Targets
* Tier Wise Performance Targets
* NFR Dimensions to be considered (samples provided below)
  * Availability
  * Reliability
  * Security
  * Recovery
  * Usability
  * Maintainability
* Conclusion
This isn’t meant to be an exhaustive list of what you might need to need to put into a Non Functional Requirements Document but rather a list of areas you might consider focusing on. Feel free to come back to us with your thoughts and input on any important sections which you think we might have left out of this Table of Content.

### Let’s Create A Few Non Functional Requirements

Now that we have got this far let’s take some time to go through a few example with regards to real world Non Functional Requirements.

* The response time for the submit order transaction should be no more than 4s for 90th percentile of users
* The system should be able to sustain a peak user concurrency of 10,500 users for the documented workload (this assumes you have a workload model that talks about the various transactions/hr, messages/hr, batch jobs/hr, etc. that the system supports)
* The application CPU utilization for the agreed workload and user concurrency should be no more than 40% at peak. This should allow for a failover scenario where the system is able to sustain workload in absence of the second application server.
* The RTO or Recovery Time Objective for the system is 8 hours.

### Conclusion


Through this document we’ve covered the importance of Non Functional Requirements, how NFR’s are aligned with performance budgets, how NFR’s are designed, the different dimensions for NFR’s and how NFR’s are measured/implemented across the delivery life cycle. This HowTo’s like most others at Practical Performance Analyst is a living document. We encourage you to send through any feedback, review comments and input you might have. Drop us a note with your thoughts or use the comments below to help us improve the HowTo.

