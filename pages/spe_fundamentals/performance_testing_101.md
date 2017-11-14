---
layout: pagelayout
title: Performance Testing 101
---

This section will define the concepts of Application Performance Testing and delve into details around Performance Testing as seen from the eyes of the Practical Performance Analyst (some one like yourself). The topics we intend to cover in this section are –

* What is Performance Testing
* Why is Performance Testing Important
* Pre-requisites for Performance Testing
* When should i Performance Test
* Types of Performance Test
* Activities involved in Performance Testing
* Challenges involved in Performance Testing
* Deliverables from the Performance Testing Process
* Evaluation criteria for selecting Performance Testing tools
* Tools for Performance Testing
* Resources on Performance Testing

### What is Performance Testing

So lets start by taking a look at what is Performance Testing and how it fits within the overall scheme of Systems Performance Engineering. 

Performance Testing is the process of validating your application Performance and Scalability against documented Non Functional Requirements with the objective of understanding the end user experience (or also called End User Customer Experience). Performance Testing can go under different names, i.e.

* Stress & Volume Testing
* Performance & Volume Testing
* Performance Benchmarking

However, the objective of Performance Testing is always to identify the Performance and Scalability limitations of your application with regards to documented Non Functional Requirements. In some cases where Non Functional Requirements don’t exist (and I won’t be surprised to know that there will be quite a few of you who know of such applications) Performance Testing would be about validating the point beyond which the application performance tanks.  In the forthcoming section we will look at the different types of Performance Tests, their definitions and their objectives. 

As you’ve realized, benefits of Performance Testing would be truly realized when the following components are addressed before you start doing any real performance tests –

* Define your non Functional Requirements
* Document your Performance Testing Workload (Transaction mix, transaction types, etc.)
* Define the problem statement, identify the program goals and define your Performance tests accordingly

### Why is Performance Testing Important

Performance Testing is important for several reasons.

* **Proactively identify application bottlenecks** – One of the most common uses of Performance Testing is to proactively identify application bottlenecks across the SDLC. As a Practical Performance Analyst you would be working closely with the application development teams, testing parts of the application validating the Non Functional Requirements and identifying any potential performance issues across the various application tiers. Proactive Performance Testing helps minimize defects during the end to end Performance Testing Cycle and helps the performance testing team focus on tuning and optimization of the application later in the development cycle.
* **Proactively identify application breaking point** – Many a times we find ourselves in a situation where customers have made modifications to a given application stack i.e. upgraded the underlying application container, changed the container configuration setting, upgraded the underlying hardware, upgraded the underlying networks, etc. but don’t have a clue about the change in application performance.  In such cases as a Practical Performance Analyst you would recommend validating the change in application performance by testing for the documented workload by executing the relevant Performance and Stress tests. Identifying the application breaking point helps business understand the Performance & Scalability limitations of the underlying platform and potential barriers to business growth while giving the development teams and performance testing teams an opportunity to assess their current position and the effort required to get the application to meet the documented Non Functional Requirements.
* **Validate documented Non Functional Requirements** – This by far is the most common use of Performance Testing where the Performance Testing team validates application performance and scalability against the document Non Functional Requirements by subjecting the application to the document user workload (OLTP, Batch, Workflow, Messaging, etc.). As mentioned earlier Performance Testing can be proactive (early in the development life cycle) or re-active (at the end of the development process just before go live) and the benefits derived out of Performance Testing is completely dependent on the amount of effort put into in to planning through Performance Tests.
* **Document business workload processing limitations** – As mentioned earlier, as part of determining performance and scalability limitations as a Practical Performance Analyst you would like to be able to communicate to business the scalability of the underlying application platform. You can design Performance tests such that they validate the breaking point of the platform by establishing the point beyond which End User Application performance is un-acceptable or breaches the documented SLA’s (Service Level Agreements).
* **Establish a Performance & Scalability Baseline** – Designing a new application or a new business initiative is very exciting. But what also is more exciting is that as a Practical Performance Analyst you now have the opportunity to establish the Performance & Scalability baseline for the application and validate it against the documented Non Functional Requirements with the objective of tuning the application to meet your Performance & Scalability targets. As a Practical Performance Analyst you would also recommend baseline activity when you are brought on to identify Performance & Scalability constraints of an existing application platform for which no Non Functional Requirements, Performance Testing Results or Capacity Plans are available. Establishing a Performance Baseline helps you determine where you currently stand and identify an approach to meeting the customer’s Performance & Scalability requirements.
* **Provide feedback to the development teams** – Proactive Performance Testing is the best way to identify bottlenecks early on in the SDLC. This gives the development teams the opportunity to revisit the code as it is being developed and fix issues at a lower cost. Having said this is also quite tough to achieve during an extended release as part of the normal waterfall model. It takes a lot of perseverance and agreements with all the business and IT stake holders to agree to proactive Performance Engineering across the early part of the SDLC. Agile development is quite different where each cycle of activity requires thorough performance testing of small part of application functionality this limiting the change required from a design and optimization standpoint towards meeting your documented Non Functional Requirements.
* **Validate impact of design or code changes for a given release** – Validating the impact of functional changes is another reason why customers like to validate the application Performance & Scalability. Ideally you have an existing suite of Performance Testing Scripts for the documented Non Functional Requirements and Workload which can be injected through the application to determine the change in application Performance & Scalability.

As a Practical Performance Analyst stay focussed on the business outcomes. Yes, Performance Testing is cool and its really engaging but try to keep reminding yourself of the end goals. The customer has limited funds and you are there to ensure the funds are utilized in the most optimal manner to deliver maximum bang for the buck. Don’t test for the sake of testing but test to validate Performance & Scalability with a clear understanding of the business objectives and goals.

### What are the Pre-requisites for Performance Testing

The pre-requisites for Performance Testing are as follows-

* Understand the business objectives
* Document the Non Functional Requirements & obtain sign off
* Document the Performance Testing Workload & obtain sign off
* Document the Performance Testing plan & obtain sign-off
* Identify the infrastructure requirements for Performance Test
* Identify the appropriate Performance Testing & Performance Monitoring tools
* Identify the appropriate Diagnostics tools required to identify Performance bottlenecks during performance test
* Identify the appropriate analysis tools required to assess the realms of data generated during performance test
* Instrument the application with the appropriate performance monitors (Operating System, Application, Network, etc)
* Create your Performance Testing Scripts
* Design your Performance Testing Scenarios

The above list doesn’t aim to cover every scenario that you might encounter but rather a set of guiding principles that you could refer to every time you are tasked with Performance Testing your applications.

### When should I Performance Test

As a Practical Performance Analyst your job as the chief risk mitigation officer is to identify opportunities for Performance Test across the SDLC with the objective of proactively identifying performance bottlenecks and validating Performance & Scalability limitations for the documented Non Functional Requirements. Here’s a list of possible scenarios when you should consider validating your application performance and scalability.

* Early on in the design phase to validate the design principles
* Through the development life cycle to identify potential performance bottlenecks
* Before go-live to validate the Performance & Scalability against documented Non Functional Requirements
* Validate the effect on Performance & Scalability due to functional changes
* Validate the effect on Performance & Scalability due to change in configuration or change in infrastructure specifications
* Need to establish a Performance Baseline to identify the breaking point of the application and communicate to business the TTL (Time To Live)

The best approach to minimizing risk across the SDLC is to performance test early and performance test often. However performance testing without a good understanding of the business requirements, the Non Functional Requirements, the business workload, etc. would only lead to useless performance testing results. Performance Testing is an art and there is enough of documentation available around the web to train yourself on becoming a skilful artist and a strong practicing Practical Performance Analyst.

![Performance Testing Modelling Process]({{ "/assets/img/performance_testing_process.png" | absolute_url }})

### What are the different types of Performance Tests 

The types of Performance tests you would design as part of your Performance Testing approach would squarely depend on the business objectives, goals and the Non Functional Requirements. The various type of performance tests are summarized below-

* **Load tests** – Determine performance and scalability of the system by subjecting it to a given workload. Your objective here is to assess end user performance for a given user workload and a set of Non Functional Requirements.
* **Soak tests** – Determine performance and scalability of the system by subjecting it to a given workload for an extended time period. The objective of this test is to determine system behaviour and end user performance when the SUT (System Under Test) is subjective to a given workload for an extended period of time.
* **Break point tests** – Determine breaking point of the system for a given system configuration. Breaking point is generally defined as the workload beyond which the end user experience for a given application crosses the documented SLA’s. Break point tests are usually performed to identify performance & scalability limits of the application with the objective of identifying opportunities for tuning and optimization.
* **Volume tests** - Volume tests involve scaling the amount of data in the data stores (Databases, file stores, etc.) used by the application to the maximum expected sizes (over the course of the life of the application e.g. xx TB over 10 years as specified in the Non Functional Requirements) and validating performance of the system for that scenario.
* **Stress tests** - Stress tests include design and execution of test conditions where the workload (user concurrency, threads, etc.) on the system is suddenly increased to expected peak including potential conditions where the workload volumes then drop to expected troughs. 

The above list doesn’t aim to cover every scenario that you might encounter but rather a set of guiding principles that you could refer to every time you are tasked with Performance Testing your applications. In most cases based on the stated business objectives and goals you’ll find yourself designing performance testing approaches that use a combination of different test types towards validating the documented Non Functional Requirements.

### What are the activities involved in Performance Testing –

The activities involved in Performance Testing are as follows –

* Understand business objectives and goals
* Document Non Functional Requirements
* End User Performance (Response Times, Page Load Times, etc.)
* Application Performance (Throughput, Txns/Sec, etc.)
* System SLA’s (System Utilization targets, Container utilization targets, etc)
* Availability & Reliability requirements
* Document Performance Testing Workload
* Transaction mix
* Transaction SLA’s
* Transactional throughput
* Document Performance Testing Plan
* Document Infrastructure Requirements for Performance Test
* Document Performance Testing tool requirements
* Document Performance Monitoring tool requirements
* Document Application Diagnostics tool requirements
* Document Data Analysis tool requirements
* Create Performance Testing Scripts and test data volumes
* Create Performance Testing scenarios
* Instrument application with monitors
* Execute Performance tests and identify opportunities for optimization
* Tune, optimize and re-execute tests to validate effect of changes

Performance testing is an iterative process where you as the Practical Performance Analyst help the business and customer define their goals and work through a rigorous approach towards validating those goals using a set of defined processes and tools.

### What are the challenges involved in Performance Testing – 

Performance testing like any other activity in Performance Engineering is fraught with challenges. As a Practical Performance Analyst, being aware of these challenges and knowing how to deal with them is critical to your success on any performance testing engagement.

* Lack of documented Non Functional Requirements
* Lack of data to create Performance Testing Workload
* Lack of Business SME’s required to create Non Functional Requirements
* Lack of Application SME’s to analyse application data for Workload analysis
* Lack of budget for Performance Testing, Monitoring, Diagnostics and Analysis tools
* Lack of capable and experienced Performance Testing Engineers
* Lack of capable and experienced Diagnostics and tuning engineers
* Gaps between production environment infrastructure specifications and performance testing environment infrastructure specifications
* Lack of time to execute a thorough performance test
* Lack of business and customer buy in for a thorough performance test
* Lack of application knowledge and challenges with tuning and optimization
* Lack of performance maturity across the customer leading to reactive performance testing requests

As a Practical Performance Analyst you’ll be tasked with delivering the impossible. You’ll be tasked with leading a monumental effort and the expectations are generally huge. Inevitably during performance test one or more of the above scenarios would be true and you would be expected to work with one or most probably several of the above constraints. The challenge will always be how do I balance risk v/s rewards, what do I recommend as a suitable performance testing approach fully knowing the challenges and constraints that I have to work with, how do I execute on-going performance tests fully knowing the constraints you have to work within.

Performance Testing is interesting, challenging and is an art. As a Practical Performance Analyst you have to train yourself on being practical and identifying the right strategy by having an excellent understanding of the business requirements, Non Functional Requirements, Performance Testing Workload and recommending an approach based on good understanding of the customers risk appetite.

There’s nothing perfect in this world and it’s amazingly rare that you’ll ever come across a customer who has the performance maturity level, perfect environment, perfect set of tools, perfect set of resources, perfect set of application and business SME’s, perfect set of timelines and a perfect understanding of what needs to be done. You’ll be called up time and time again to step out of the box and be creative in designing an approach that delivers the performance testing results the customer expects to see with a combination of different constraints.

Your effectiveness in delivering such an engagement will test your nerve and your ability as a Practical Performance Analyst.

## Deliverables from Performance Testing process

The deliverables from the Performance Testing process are listed below –

* Non Functional Requirements
* Performance Testing Workload
* Performance Testing Strategy & Plan
* Performance Testing results

This section will eventually include links to templates for each of the above deliverables.

### Evaluation criteria for selecting Performance Testing tools 

When selecting Performance Testing tools you would want to be looking out for the following –

* Does the tool support your application protocol(s)
* Does the tool scale to your performance testing needs (Virtual User needs)
* Does the tool integrate with performance monitoring and diagnostics tools
* Does the tool provide intuitive interfaces to export and analyse test results
* Does the tool or vendor provide you a SaaS option allowing you to execute tests from the cloud
* Does the tool vendor have capability on the ground to support your performance testing needs

### Tools for Performance Testing

Performance Testing tools have been largely dominated by commercial solutions and generally tend to have a very clear focus i.e. the tool could be either focused on Application Performance Testing or Infrastructure Performance Testing with a clear view of the platforms or protocols they would support. A handful of the industry standard Performance Testing tools have extensive support for a very large number of different application protocols while the rest of the tools have limited support and are largely focused on web based applications. A list of Performance Testing tools is provided below.

* HP Load Runner – [Link](http://www8.hp.com/us/en/software-solutions/software.html?compURI=1175451)
* IBM Rational Performance Tester – [Link](http://www-01.ibm.com/software/awdtools/tester/performance/)
* Microsoft Visual Studio Ultimate Edition – [Link](http://www.microsoft.com/visualstudio/en-gb/products)
* Webload – [Link](http://radview.com/)
* Neoload – [Link](http://www.neotys.com/)
* Load Storm – [Link](http://loadstorm.com/performance-testing-tool)
* Micro Focus Silk Performer – [Link](http://www.microfocus.com/products/silk/silkperformer/index.aspx)
* SOASTA Cloud Performance Test – [Link](http://www.soasta.com/)

### Resources on Workload Modelling

* [Wikipedia](http://en.wikipedia.org/wiki/Software_performance_testing)
* [Performance Testing Blog](http://www.perftesting.co.uk/)
* [Alexander Podelko’s Blog on Performance Engineering](http://alexanderpodelko.com/blog/)
* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)

### Additional Resources

Here’s a list of important resources on Performance Engineering :

* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

