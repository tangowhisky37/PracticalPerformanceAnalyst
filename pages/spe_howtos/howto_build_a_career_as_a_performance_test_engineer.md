---
layout: pagelayout
title: Howto Build A Career As A Performance Engineer
---

Welcome to the How-To on Building A Career as a Performance Testing Engineer.

The topics covered in this HowTo are:

* Introduction
* What are HowTo’s
* Why HowTo’s @ PPA
* Why We Wrote, HowTo Build A Career As a Performance Testing Engineer
* What is Performance Testing
* How does Performance Testing fit into the overall Performance Engineering life cycle
* What are the different types of Performance Tests
* Why do businesses consider investing in Performance Testing
* Why is Performance Testing challenging and exciting at the same time
* What are the various activities involved in delivering a Performance Test
* Why one might consider Performance Testing as a profession
* What are the career paths for someone who would like to consider sticking to Performance Testing as a specialization
* What are some of the skills a Performance Testing Engineer might want to invest in
* What are some of the leading Performance Testing tools a Performance Engineer might want to invest in learning
* What are different types of opportunities one might want to focus on
* What are some of the recommended reads for someone interested in Performance Testing
* Where could my Performance Testing career lead me
* Conclusion

### Introduction

Software Performance Engineering or SPE prescribes a set of processes, activities, roles, responsibilities and deliverables across the Development Life Cycle with a view to proactively managing system performance. Among the various activities prescribed within SPE (Systems Performance Engineering) Performance Testing focuses on validating system performance. Performance Testing, as an activity can be performed across the delivery cycle as a proactive or reactive task depending on the outcomes desired and the way the program or organization is structured. This document is not intended to be a Performance Testing HowTo as such but rather a document that provides a view on the opportunities for a Performance Testing Engineer, skills required to become a Performance Testing Engineer and what approach one might consider when wanting to build skills required to be a strong Performance Testing Engineer.

### What Are HowTo’s

A HowTo is a document that does precisely what the name suggests i.e. It’s describes “HowTo” achieve a set of outcomes through illustration of all the steps involved. HowTo’s are generally structured and written without too much technical jargon in a straight forward manner without making too many assumptions of the depth of knowledge the reader. HowTo’s are meant to make for easy reading and are logical in the sequence of steps it recommends.

Any background knowledge required to assimilate the information provided in the HowTo is generally highlighted at the start of the HowTo. HowTo’s are generally written for the professional who are clear of what they need to accomplish but have little or no knowledge of how to go about achieving those objectives. HowTo’s are meant to be exhaustive in nature and they are definitely not meant to offer the most efficient way of getting the job done. A  HowTo should be seen as a kick starter that helps the user get up and running with a given task without having to master all the required fundamentals.

### Why HowTo’s @ PPA

HowTo’s have been the mainstay of the Open Source and Free Software movement for decades. One of the reasons why Open Source and Free Software is so widely used today is simply because of the depth of documentation that exists and the maturity of the Open Source ecosystem which has delivered scalable, open and reliable software. HowTo’s like many other building blocks have helped the Open Source and Free Software movement grow immensely while eliminating the need to keep re-inventing the wheel. It’s only natural that we at Practical Performance Analyst adopt the best from the Open Source and Free Software movement. A lot of the work we do at Practical Performance Analyst borrows from the fundamentals of the Open Source movement and HowTo’s are definitely one of them.

As HowTo’s @ PPA grows and matures we will hopefully reduce the reinventing of the wheel which happens so very often at organizations, projects and programs when it comes to the science of building/delivering systems that scale.

### Why We Wrote, HowTo Build A Career As A Performance Testing Engineer

SPE (Systems Performance Engineering) has traditionally been a very poorly defined science with lack of clearly defined processes across the delivery life cycle. Within the SPE (Systems Performance Engineering) life cycle though Performance Testing is possibly one of the most well know disciplines. However Performance Testing also very often seems to be one of the most poorly implemented disciplines when it comes to rigor from an implementation/delivery standpoint. Performance Testing is traditionally also known to one of the most expensive activities a program needs to invest in given the costs involved along the following dimensions  –

* Costs of a production like environment for purposes of executing a meaningful performance test
* Costs of experienced Performance Testing resources
* Costs of experienced Performance engineering resources
* Costs for relevant Performance Testing tools
* Costs for relevant Application & System Diagnostics & Monitoring tools
* Costs for Application SME’s to tune and fix performance issues across the system
* Delays to the program due to the engineering required to get the system to scale and meet the overall Non Functional Requirements

Performance Testing overall is not rocket science and when implemented sensibly it can deliver the expected outcomes, any experience Technical Architect or Performance Engineer would tell you that. What’s required is diligence with regards to the approach for Performance Testing along with relevant investments in putting together the required deliverables to execute a useful Performance Test. We’ll cover some of these later in this document.

The objective of this HowTo titled, “HowTo Build A Career As A Performance Testing Engineer” is to help the reader understand the following –

* What does the role of a Performance Testing Engineer look like
* What are the common activities involved in Performance Testing
* What are the skills required for Performance Testing
* What are some of the reasons one would want to invest in becoming a Performance Testing engineer
* How does the pay for a strong and experienced Performance Testing Engineer compare with that of an strong and experienced Developer or Solution Architect
* How does investment in Performance Testing skills go towards building skills in others areas of Performance engineering

The changing circumstances and the world we live in today recommends adoption of various agile development techniques along with Continuous Integration, DevOps, etc. where the emphasis is not on developing the best or most scalable solution but rather designing a solution that works and getting it out there, iterating as teams move along learning from experiences on the field. The shortening of the development iteration leaves the average Project or Program Manager with not enough time, human resources or money to put together a useful Performance Test. These are some of the realities which the Technical Architects and Performance Engineer of today has to deal with.

One of the big challenges of anyone aspiring to become a Performance Testing Engineer will eventually face is getting their customers/organizations to invest in doing the job well and not just doing the job. As a Performance Engineer you have to go in with your eyes wide open not expecting a perfect scenario but rather expecting a broken one where you do what you can with the limited resources on hand to help deliver a system that’s engineered to scale and meet the agreed Non Functional Requirements.

### What is Performance Testing

Performance Testing is the process of validating the ability of the system to meet the relevant Non Functional Requirements. (This document will not go into the details of Non Functional Requirements or NFR’s but if you are interested in knowing more about Non Functional Requirements or NFR’s we would suggest checking out some of the other HowTo’s at the HowTo section here at Practical Performance Analyst. One of the more relevant HowTo’s that focus on Non Functional Requirements is – HowTo Define Non Functional Requirements). You can access the HowTo’s section through the following [link](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_fundamentals/performance_testing_101/).

To be able to validate Performance for a given system as a Performance Engineer or a Performance Testing Engineer you need to have a good understanding of the relevant Non Functional Requirements e.g. Scalability, Performance, Reliability, High Availability, Failover, etc. and the applicability of the Non Functional Requirements (NFR’s) to the overall functional requirements. Understanding of the Non Functional Requirements (NFR’s) is great but to be able to deliver a system that scales and meets the functional expectations you would like to make sure you understand some of the key functional criteria for the agreed Workload (Transactions, Batch jobs, Reports, Messages, etc.) for which you are on the hook to meet the agreed Non Functional Requirements (NFR’s).

With knowledge of the relevant Non Functional Requirements (NFR’s) you can then design the relevant Performance Tests aimed and validating the Performance of the system as a whole or Performance of a given Tier within the system.

The outcomes of Performance Testing would depend on what you want to get out of the test i.e.

* During the initial build phase when you do not have an integrated Performance Testing system available you might consider designing a Performance Test that could validate the performance of a component of the given system.
* During the initial build phase when you do not have an integrated Performance Testing environment available another good approach involves getting developers to design unit tests to test out the code they are writing which can be used to both validate the code delivered functionally and from a performance perspective.
* When the system has got to a stage where the various components are now functionally stable and are able to talk to each other you might consider building and executing an integrated Performance Test
* When the entire system has been built, is functionally stable and has completed Integration Testing you might considering executing an End to End Performance Test to understand how the entire system behaves for different aspects of the workload.

Performance Testing in essence consists of injecting relevant workload into the system to understand how your system will stack up when it goes live and has to deal with real customers pushing through real transactions in a live system. Injection of the Workload into the system can be performed using industry standard Performance Testing tools like HP Load Runner, HP Performance Center, Neoload, Webload, etc. or Open Source tools like Jmeter, Grinder, etc.  Workload in our case is the work that is done by the system and consists of Transactions, Batch Jobs, Messages, Workflows, Messages, etc. With a good understanding of your Workload combined with an understanding of the user behavior you can design sensible Performance Tests that inject workload into the system to help you understand how the system will stack up.

In essence Performance Testing is a risk mitigation process. The more the effort you put into setting up your Performance Engineering processes including the Performance Testing processes across the program, the more likely that you will end up with relevant outcomes when the system goes live. In a digital world where systems are connected all the time and customers expect seamless transition of experiences with your products/service not investing in the relevant Non Functional attributes can put your business model in peril.

### How does Performance Testing fit into the overall Performance Engineering life cycle

Software Performance Engineering or SPE prescribes a set of processes, activities, roles, responsibilities and deliverables across the Development Life Cycle with a view to proactively managing system performance. Among the various activities prescribed within SPE (Systems Performance Engineering) Performance Testing focuses on validating system performance with the objective of understanding the ability of the system to meet the agreed Non Functional Requirements or NFR’s. Performance Testing the way it has traditionally been looked at has been reactive in nature i.e. Performance Validation performed on the system once the integrated system is available for an End to End Performance Test, but the good news is that it doesn’t really have to be that way.

Performance Testing, as an activity can be performed across the delivery cycle as a proactive or reactive task depending on the outcomes desired and the way the program or organization is structured.

The various activities in a Performance Engineering cycle for a given project can be defined as follows –

* Definition of the Performance Engineering Approach
* Definition of the overall Non Functional Requirements (NFR’s)
* Definition of the Performance Testing Approach
* Definition of the Workload Model for Performance Testing, Capacity Management
* Definition of the Capacity Plans including Performance Models
* Execution of the Performance Tests – Component, Integrated, etc.
* Performing Application/System Monitoring, Triage and Diagnostics to optimize the system
* Perform on-going Monitoring, Capacity Management & Performance Modelling

Overall the Performance Engineering life cycle is focused on helping build a system that stacks up to the expected Non Functional Requirements or NFR’s. The Performance Testing activities within the Performance Engineering Lifecycle (whether executed proactively or re-actively) help validate the ability of the system to meet those agreed Non Functional Requirements or NFR’s.

We stress on the dual interpretation of Performance Testing as a proactive or re-active activity within the Performance Engineering life cycle. The broad adoption of DevOps, Agile software development methodologies, Continuous Integration, etc. could very well have Performance Testing integrated so as to proactively be validating the performance of the system very early on in the development process. In contrast when you view Performance Testing from the lens of a project that is delivering a system through some form of a waterfall based model Performance Testing inevitable becomes a reactive process and ends up validating system performance once all the defects (architectural, code, etc.) have been baked into the system.

### What are the different types of Performance Tests

This section lists down some very common types of Performance Tests which you will come across. Please do note that due to lack of a universally acceptable lingo for Performance Engineering the names of the various activities within Performance Engineering and Performance Testing in general will vary depending on whom you speak to across the industry and their knowledge of Performance.

* **Load Tests** – Load tests are Performance Tests where an agreed workload (Mix of transactions, Batch jobs, Messages, Workflows, etc.) are injected into the system and the behavior of the system is monitored for the duration of the performance test.
* **Stress Tests** – Stress tests are Performance Tests where an agreed workload (Mix of transactions, Batch jobs, Messages, Workflows, etc.) is injected into the system such that the workload injected includes multiple peaks and troughs. The intention of injecting a workload mix that includes a mix of peaks and troughs in succession (with possible gaps) is to subject the system to possible conditions it might experience in production where there is a sudden surge of customer traffic into the environment.
* **Soak Tests** – Soak tests are Performance Tests where an agreed workload (Mix of transactions, Batch jobs, Messages, Workflows, etc.) is injected into the system over an extended duration e.g. 8 hours, 16-24 hours, etc. The objective of soak tests is to understand performance of the system over an extended duration of time.
* **Volume Tests** - Volume tests are types of performance tests where the system is setup with extremely large volumes of data in the databases, message queues, data stores, file system, etc. to validate the behavior of the system 5-7 years down the line.

To learn more about performance tests and how Performance Testing fits within the overall Performance Engineering life cycle please visit [Link](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_fundamentals/performance_testing_101/). With a basic understanding of the various Performance Testing types in the background you can see that Performance Testing involves some really interesting challenges. Performance Testing unlike functional testing requires a good understanding of the business objectives including the technical acumen to understand the complexity of the technical architecture (for the solution being proposed), understand the existing Non Functional Requirements (NFR’s) to be able to put together a sensible Performance Testing approach.

The combination of Performance Tests for a given program will completely depend on the Non Functional Requirements (NFR’s) the program is on the hook to meet.

### Why is Performance Testing challenging and exciting at the same time

Finally we’ve come to one of the most important sections of this document i.e. Why is Performance Testing a compelling Career option for any techie. Performance Engineering is generally considered a black art which lacks a generally accepted Body Of Knowledge (This is something we are changing at Practical Performance Analyst) along with lack of defined processes/activities that organizations might invest in across the System Development Life Cycle. This is probably one of the reasons why seasoned Performance Engineers speak in languages that sometimes do not make sense to each other.

Before we dive into some of the more exciting parts of Performance Testing let’s look at the various activities involved in Performance Testing across the System Delivery life Cycle –

* Document the Non Functional Requirements or NFR’s
* Document the Performance Testing Approach
* Document the Workload model
* Design the Performance Testing Scripts using the Performance Testing tool
* Sort out the data dependencies, environment requirements, etc.
* Design the workload model using the Performance Testing Tool
* Inject the workload into the system
* Monitor System Performance, Application Performance, etc.
* Triage performance issues using Diagnostics tools, monitoring tools, etc.
* Raise defects and work with the engineering, build team to tune/optimize the system
* Feed learning back into step 1

As you would note from what we’ve just listed above there’s a set of sequential steps one would perform to get their performance tests up and running. However, the objective of a Performance Test is not to test the system but identify areas of optimization across the board, identify tuning/optimization activities and work with the Engineering/Build teams to deliver a system that scales and meets the documented Non Functional Requirements. Performance Testing is truly an Engineering activity which touches upon various other activities across the Performance Engineering Life Cycle. 

Some of these activities include –

* Verifying the capacity plans for the infrastructure the system is built on
* Application Performance Monitoring, Infrastructure Performance Monitoring, etc.
* Diagnostics, Application Profiling, etc.
* Performance Modelling based on empirical data you’ve collected from the performance tests, etc.

Performance Testing thus as you would have realized is not just about consuming the NFR’s that the Business Analyst has provided, putting together workload, designing the scripts and injecting the workload into the system only with the objective of coming up with a lovely report that lists down the various performance bottlenecks across the system. Performance Testing is truly an Engineering exercise where the Performance Testing engineer works closely with other parts of the application development, infrastructure design/build team, storage team, networking team, etc. to put together a set of sensible performance tests and work with these individuals to identify bottlenecks across the system so that the system can be tuned/optimized to meet the agreed Non Functional Requirements.

Finding defects and bottlenecks is interesting and challenging for sure but the real fun is working with the architects, development leads, infrastructure engineers, storage engineers, network experts, etc. to identify solutions to various engineering or architectural issues across the system. Performance Testing can be as challenging as you want it to be, look at it as an Engineering exercise where you deliver outcomes rather than just a testing process that spins up scripts to inject workload into a system and deliver a glossy report that few within your development or build team can make sense of.

### Why do businesses consider investing in Performance Testing

Organizations consider investing in Performance Testing since it’s a risk mitigation approach which helps the business identify bottlenecks, configuration issues or architectural issues that could impact the End User Experience when the system goes live. In a digital world where the customer today expects a seamless End User Experience across different devices types i.e. mobile, PC, tablet, etc. few businesses can afford to not cater to a great customer experience. Businesses who do not invest in performance are obviously doing their best to give their competitors and advantage and possibly also leaving a lot of cash on the table.

### What are the various activities involved in delivering a Performance Test

A Performance Testing project could include some or all of the activities listed below –

* Document the Non Functional Requirements or NFR’s
* Document the Performance Testing Approach
* Document the Workload model
* Design the Performance Testing Scripts using the Performance Testing tool
* Sort out the data dependencies, environment requirements, etc.
* Design the workload model using the Performance Testing Tool
* Inject the workload into the system
* Monitor System Performance, Application Performance, etc.
* Triage performance issues using Diagnostics tools, monitoring tools, etc.
* Raise defects and work with the engineering, build team to tune/optimize the system
* Feed learning back into step 1

Performance testing in the agile world can mean different things to different teams and organizations. In the DevOps context where a team might have Continuous Integration built into the delivery processes Performance Testing is probably baked into the core Quality Assurance processes. On other projects where a business is embarking on a green field initiative Performance Testing might consist of the following activities –

* Unit performance tests
* Tier wise performance tests
* End to End or integrated performance tests

Performance testing is interesting and challenging due to the nature of technical tasks involved and the demand from the Performance engineer to be able to communicate to business the value and outcomes of a Performance Test.

### What are the career paths for someone who would like to consider sticking to Performance Testing as a specialization

There are various career paths one could consider taking on within the Performance Testing space –

* **Performance Testing Engineer** – A Performance Testing Engineer would be responsible for all the technical performance testing activities on a program. This would ideally involve Workload Modelling, Scripting, Scenario Design, Script Execution, Data Creation, Results Analysis and assisting the Build, Development, Operations team with the triage required during and after the test runs.
* **Performance Testing Lead** – A Performance Testing Lead is usually a very experienced Performance Testing engineer who has been hands on in the past, understands the process end to end and is able to work with business, architecture, development, infrastructure, operations, etc. to design relevant performance tests, drive the required Non Functional outcomes and lead the overall Performance Testing team. A Performance Testing Lead usually has
* **Performance Diagnostics & Monitoring Engineer** – A Performance Diagnostics & Monitoring Engineer is usually an SME with APM (Application Performance Monitoring) and Diagnostics experience. This is usually an individual with prior development experience i.e. Java, .Net, C#, etc. and the ability to use APM (Application Performance Monitoring) and Diagnostics tools to identify performance bottlenecks across the system while the Performance Testing team is injecting workload across the system.
Some of the other supporting roles within a Performance Testing team are –
* **Environment manager** – Responsible for managing and maintaining the infrastructure required for Performance Test
* **Data Management Expert** – Responsible for putting together the data requirements for Performance Test, managing the data extraction process and tracking data requirements for all the systems across Performance Testing.
* **Defect coordinator** – Responsible for raising and managing defects across the Performance Testing cycle.
* **Technical Project Manager** – Responsible for managing the overall Performance Testing deliverables, tracking to schedule, managing the execution of Performance Testing activities and reporting to the program on the progress (or lack of it).

The roles listed in this section are by no means a comprehensive set of roles you will find in the Performance Testing space but should provide a view of some of the most commonly found roles within the Performance Testing team. A strong Performance Engineer would look to play a combination of the above roles across a wide variety of application platforms using a variety of Performance Testing, APM (Application Performance Monitoring) and Diagnostics tools.

### What are some of the skills a Performance Testing Engineer might want to invest in 

Let’s take a brief look at some of the skills a strong Performance Testing Engineer might want to invest in. The intention here is not to start a flame war but rather to give you a view of the most relevant skills required to be strong Performance Testing Engineer –

* Have an inquisitive attitude
* Never accept no for an answer
* Learn to fail quickly, cheaply and often
* Understand the basics of Operating Systems (We would highly recommend you pick up a Linux distro and start hacking)
* Understand the basics of communication protocols and how they work i.e. TCP/IP, UDP
* Understand the basics of how Virtualization works i.e. in the context of Vmware, Xen, etc.
* Understand the basics of how Private Cloud, Public Cloud and Hybrid Cloud works
* Understand the concepts required to put together Non Functional Requirements
* Understand the concepts required to put together Workload Models
* Pick up some relevant Data Analytics skills, very useful in analyzing realms of text data obtained from application/system logs
* Take a refresher and strengthen your understanding of the basics of Statistics
* Build an understanding of the use of Statistical Modelling & Forecasting tools
* Understand the concepts required to put together a Performance Testing Approach
* Understand the process of Performance Testing
* Get your hands dirty with some of the following Performance Testing tools
  * Jmeter
  * Neoload
  * HP Load Runner
  * Web loadhttps://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_fundamentals/performance_testing_101/
* Get your hands dirty with some of the following monitoring tools –
  * Nagios
  * Zabbix
  * Zenoss
  * MS PerfMon
* Get your hands dirty with some of the following Diagnostics and APM (Application Performance Monitoring) tools –
  * AppDynamics
  * New Relic
  * Dynatrace
  * Yourkit
* Get your hands dirty with some of the following Log Analysis tools
  * Splunk
  * Sumologic
  * ELK (Elastic Search – Logstash – Kibana)
* Have an insatiable desire to learn and make the world a better place

Think of Performance Testing as a process who’s objective is to rid the world of poor performing systems. Systems that perform better increase productivity overall, make for happy customers and hence make for happier employees.

### What are some of the leading Performance Testing tools a Performance Engineer might want to invest in learning

In the previous section we touched very briefly on some of the most commonly used Performance Testing tools in the industry. The intention here is not to start a flame war as such and neither are we being paid manufacturers to promote their tools. This list is not intended to be comprehensive in nature but rather reflects a subset of the industry leading tools one might consider when looking at building Performance Testing skills.

* Jmeter (Open Source)
* Gatling (Open source)
* Neoload
* HP Load Runner
* HP Performance Center
* Webload
* SOASTA (Cloud based)
* Keynote (Cloud based)

The two of the most common Open Source tools used for Performance Testing today are Jmeter and Gatling. We would encourage you to start with Jmeter or Gatling when you are just embarking on your journey towards becoming a Performance Testing Engineer. For those with some Performance Testing skills and an understanding of the Performance Testing processes you might consider downloading and using Neoload, HP Load Runner, Webload, etc.

SOASTA, the last we checked was even offering an in-house Performance Testing solution limited to 100 Virtual Users for the HTTP/S protocol.

### What are some of the recommended reads for someone interested in Performance Testing

Like more engineering skills, the true learning is in the doing. We would be kidding ourselves and you if we told you that if you did everything we said you should in this HowTo you would end up being a start Performance Testing Engineer. The reality is, everything we’ve mentioned in this HowTo is about getting you started with your move towards being a Performance Testing Engineer.

We would also recommend starting with the SPE (Systems Performance Engineering) fundamentals section here at Practical Performance Analyst. Once you are done with that we would suggest picking up projects where you have the opportunity to get some hands on experience and start building your SPE (Systems Performance Engineering) fundamentals.

### What sort of skills are recruiters looking for

When looking to move into a Performance Testing career you are probably wondering what skills are recruiters or companies looking for when the hire Performance Testing engineers. So here’s a view of some of the main skills recruiters and companies are looking for when hiring Performance Testing engineers.

* **Performance Testing Engineers** –
  * Experience working on engagements where you’ve had the opportunity to pull together a Performance Testing approach, A Workload Model, Performance Scripts, Data Requirements, etc.
  * Hands on experience with some of the industry leading Performance Testing tools
  * Experience working with the development, build and testing teahttps://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_fundamentals/performance_testing_101/ms on identifying areas of optimization across the stack
  * Experience using monitoring tools like those mentioned in the previous section to understand the performance of the system during the Performance Testing phase
  * Experience using Diagnostics and APM (Application Performance Monitoring) tools to triage the system and identify potential bottlenecks across the system
  * Experience using log analysis and data visualization tools like those mentioned in the previous system to visualize machine generated data and identify patterns that could help understands reasons for poor system performance
  * Prior development experience with an understanding of the System Development Life cycle
* **Performance Testing Lead** –
  * Prior experience working on engagements where you’ve had the opportunity to pull together a Performance Testing approach, A Workload Model, Performance Scripts, Data Requirements, etc.
  * Prior hands on experience with some of the industry leading Performance Testing tools
  * Extensive experience working with the development, build and testing teams on identifying areas of optimization across the stack
  * Extensive experience using monitoring tools like those mentioned in the previous section to understand the performance of the system during the Performance Testing phase
  * Extensive experience using Diagnostics and APM (Application Performance Monitoring) tools to triage the system and identify potential bottlenecks across the system
  * Extensive experience using log analysis and data visualization tools like those mentioned in the previous system to visualize machine generated data and identify patterns that could help understands reasons for poor system performance
  * Prior development experience with an understanding of the System Development Life cycle
  * Proven ability to lead Performance Testing teams responsible for the End to End Performance Testing process i.e. Design of the Non Functional Requirements, Performance Testing Approach, Workload models, Performance Testing Scripts, Test data creation, Test execution, Analysis, Defect triage and Reporting.
  * Ability to communicate the results of the Performance Test with program and project stakeholders.

### What are different types of opportunities one might want to focus on 

As someone aspiring to build Performance Testing skills here’s some opportunities we would recommend you take on. Again, like most other recommendations in this article these are recommendations only and it’s completely upto you to work out what’s best for you and your career.

* **Junior Performance Engineer** – Responsible for assisting with the various technical, governance, process related and documentation tasks across the Performance Engineering life cycle. This should give you a good view of the various Performance Engineering processes from Non Functional Requirements Gathering right upto Performance Testing, Capacity Management and monitoring/Diagnostics post go live.
* **Junior APM Engineer** – Responsible for setting up, configuration and implementation of the APM (Application Performance Monitoring) and Diagnostics tools. As an APM engineer you gain hands on skills learning how-to monitor applications, create performance baselines, perform triage on application components when the system performance goes awry and use the tool efficiently to help the Performance Testing / Performance Engineering team with triage of defects across the application stack.
* **Junior Performance Testing Engineer** – Responsible for assisting with the various Performance Testing related technicalities, processes, governance and related documentation. Start lower down the ladder, get as much hands on skills as you can, understand the end to end processes involved, the documentation one needs to create and the governance involved. Performance Testing as we’ve mentioned earlier is a lot more than designing relevant tests and executing them. It includes working closely with various build, development and operations leads on identifying the source of the defects and tuning the application so that it scales, performs and meets the documented Non Functional Requirements.

### What are some of the recommended reads for someone interested in Performance Testing

We would highly recommend you start by diving into the SPE Fundamentals section here at Practical Performance Analyst. Once you’ve mastered the various SPE (Systems Performance Engineering) fundamentals we would highly recommend you pick up some of the following books –

* Bob’s book on PE - The Every Computer Performance Book
* Performance Testing Guidance For Web Application - Microsoft
* The Art of Application Performance Testing by Ian Molyneaux
* Jmeter Cookbook by Bayo Erinie
* Performance Testing with Jmeter by Bayo Erinie

The list of books provided above are suggested reads. Feel free to look up various Performance Testing forums at LinkedIn, SQA Forums, etc. and hang around there to learn more about the concepts / challenges that the performance testing community is currently battling with. It should give you an idea of the kind of skills you might want to focus on if they happen to interest you.

### Where could my Performance Testing career lead me 

There’s never a boring day in the life of a Performance Testing Engineer and the reason why I say that is every day you are dealing with different sorts of challenges. If you view the role of a Performance Tester as someone who not just designs, executes, analyses the results of the tests but also as someone who works with the APM and Engineering teams to triage defects and engineer performance into the application you are assured a rewarding and challenging career.

The nature of the applications you test, the infrastructure platforms you test the applications on, the type of transactions you end up working with, the nature of the integration and backend systems you deal with, the volume of data you are dealing with, the volume of concurrent users you are injecting into the systems, etc. all combine to create a fascinating collage that’s different depending on the project you are on. Over a period of time as you strengthen your Performance Testing concepts you might start appreciating the relevance of the other disciplines across the Performance Engineering lifecycle. Depending on your interests and ability to pick up skills in the other areas of the Performance Engineering lifecycle i.e. APM, Capacity Management, Monitoring, etc. you can take chances and pick up roles in the other areas.

At-least for now, robots haven’t learned to create applications and systems that auto test and auto tune themselves. I am not suggesting that this is completely un-feasible but at-least for the foreseeable future the job of the Performance Engineer and Performance Tester shall remain highly relevant. So go forth build strong skills in Performance Testing and then try experiment with other areas across the Performance Engineering lifecycle.

### Conclusion

Performance Testing is an integral part of the overall Performance Engineering life cycle. With the move into the digital age almost every business is now a digital business. Customers are now demanding access to their data and services via seamless interfaces across a range of devices with similar performance profiles. In a world where there is no dearth of competition businesses can little afford to neglect both the functional and non-functional experiences they deliver through their applications. Performance Testing along with the other activities part of Performance Engineering will remain important for a long time into the future. The application stacks may change, the hosting providers may change, the hosting solutions may change, the consumers of the application may change but the need for applications that perform will remain.


