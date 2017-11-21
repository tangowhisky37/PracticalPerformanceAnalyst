---
layout: pagelayout
title: Howto Choose A Performance Testing Tool
---

The topics covered in this HowTo are:

* Introduction
* What are HowTo’s
* Why HowTo’s @ PPA
* Why did we write this HowTo
* What can you expect to learn from this HowTo
* Agile Testing Quadrants and Performance testing
* Why use a tool for Performance testing?
* What are the different types of Performance Tests one could perform with a Performance Testing tool?
* Does my choice of Performance Tests impact my choice of tools?
* Dimensions to consider when selecting A Performance Testing Tool
* What Are My Options: Open Source & Commercial?
* Protocol Support: What Protocol I Am Going to Need to Record My Scripts In?
* What Are the Factors That Affect Tool Licensing Models?
* What Fancy Workload Models Will I Need To Design?
* What Concurrency Should the Tool Support?
* What Scalability Considerations Should I Have In Mind?
* Does My Enterprise Need Customer Support
* How Much Is My Enterprise Willing To Spend i.e. Commercial v/s Open Source tools?
* How Much of Development Effort Are You Willing To Spend on Your Scripts (i.e. Commercial v/s Open Source tools)?
* Am I Expecting to have Automated Correlation, Parameterization & Analysis Capabilities Built into the Tool?
* Is this a Silo i.e. Project specific or an Enterprise Investment?
* What Deployment Architectures are supported?
* Does The Tool Need to Integrate with Monitoring & Diagnostics solutions?
* What Are the Training Options Available For the Tool You Are Considering?
* What Are the License Costs?
* How Strong Is the Vendor/Community Ecosystem & Vendor Support?
* Is The Tool Devops friendly and Does It Integrate with CI/CD PIPELINE?
* Conclusion

### Introduction

Performance Testing is probably the most well know of the activities across the delivery life cycle from a Systems Performance Engineering standpoint. As an activity Performance Testing focuses on validating certain (or possibly all) Non Functional attributes of the System Under Test or Component Under Test.

In this document we will focus on the need for Performance Testing, the benefits of automation, the different types of Performance Tests, and the need for tools to automate performance tests including the approach to identify a suitable tool for performance testing.

Performance Testing like most other activities part of Systems Performance Engineering is considered a black art. This HowTo along with the other information available at Practical Performance Analyst will hopefully dispel that myth and make Systems Performance Engineering a much better understood discipline.

This document is a collaboration between various SPE (Systems Performance Engineering) professionals and is completely a voluntary effort. If you find areas of improvement or have ideas, suggestions or input to make the document better please drop us a note at feedback at practical performance analyst dot com.

### What are HowTo’s

A HowTo is a document that does precisely what the name suggests i.e. It’s describes “HowTo” achieve a set of outcomes through illustration of all the steps involved. HowTo’s are generally structured and written without too much technical jargon in a straight forward manner without making too many assumptions of the depth of knowledge the reader. HowTo’s are meant to make for easy reading and are logical in the sequence of steps it recommends.

Any background knowledge to assimilate the information provided in the HowTo is generally highlighted at the start of the HowTo. HowTo’s are generally written for the professional who are clear of what they need to accomplish but have little or no knowledge of how to go about achieving those objectives. HowTo’s are meant to be exhaustive in nature and they are definitely not meant to offer the most efficient way of getting the job done. A HowTo should be seen as a kick starter that helps the user get up and running with a given task without having to master all the required fundamentals.

### Why HowTo’s @ PPA

HowTo’s have been the mainstay of the Open Source and Free Software movement for decades. One of the reasons why Open Source and Free Software is so widely used today is simply because of the depth of documentation that exists and the maturity of the Open Source ecosystem which has delivered scalable, open and reliable software. HowTo’s like many other building blocks have helped the Open Source and Free Software movement grow immensely while eliminating the need to keep re-inventing the wheel. It’s only natural that we at Practical Performance Analyst adopt the best from the Open Source and Free Software movement. A lot of the work we do at Practical Performance Analyst borrows from the fundamentals of the Open Source movement and HowTo’s are definitely one of them.

As HowTo’s @ PPA grows and matures we will hopefully reduce the reinventing of the wheel which happens so very often at organizations, projects and programs when it comes to the science of building/delivering systems that scale.

### Why did we write this HowTo

Choosing a Performance Testing tool can be a difficult process and not always are the options very clear. The options one has to consider, the implications from a costing standpoint, the implications with regards to the approach, implications with regards to skills and most important the implications to the outcomes expected are not always clear.

The content in this HowTo is aimed at helping you understand:

* Why automation is required for Performance Testing
* What options do you have when considering automation for Performance Testing
* What variables or dimensions to consider when reviewing tooling options
* What is the impact of the choice you make and how the tool can impact your ability to deliver

In a nutshell this document will help you with the thought process and approach required to help you identify a suitable Performance Testing tool for your project, business or enterprise.

### What can you expect to learn from this HowTo

Here’s the following items you can expect to learn from this HowTo:

* Why automation is required for Performance Testing
* What options do you have when considering automation for Performance Testing
* What options do you have if you are not considering automation for Performance Testing
* What is the approach to follow when reviewing tools for purposes of Performance Testing
* What variables or dimensions to consider when reviewing tooling options
* What is the impact of the choice you make and how the tool can impact your ability to deliver the expected outcomes

Performance Testing like most other activities part of Systems Performance Engineering is considered a black art. This HowTo along with the other information available at Practical Performance Analyst will hopefully dispel that myth and make Systems Performance Engineering a much better understood discipline.

### Agile Testing Quadrants and Performance testing

Performance testing is the activity undertaken to validate the responsiveness, stability and scalability characteristics of the product under a given workload. It is required to assess the production readiness of the solution and identify hotspots and sources of performance problems.

Performance testing falls in the 4th Quadrant of the Agile Testing Quadrant (popularized by Lisa Crispin and Janet Gregory). It is indicative of critiquing a product and is typically technology facing.

![Tool Selection Quadrant]({{ "/assets/img/choosing_a_tool_quadrants.png" | absolute_url }})

Fig1: Source – Lisa Crispin, Janet Gregory; “Agile Testing: A practical guide for Testers and Agile Teams”, Addison-Wesley; Jan 2009.

Performance tests are performed for various reasons across the delivery life cycle. Here are some of the common reasons why programs choose to invest in a Performance Test:

* Performance tests to determine speed and throughput characteristics
* Load tests to verify application behaviour under specific load conditions and test for scalability
* Capacity tests to determine how many users and transactions a given system will support and still meet performance goals.
* Stress test to validate a systems behaviour when subjected to load conditions that are beyond the normal range.

There are other types of performance tests like unit, component, endurance, smoke, spike etc that can be used in conjunction with the above tests to validate the performance, scalability, reliability and availability of a software solution.

### Why use a tool for Performance testing

A Performance test typically needs the ability to generate tens, hundreds or in some cases thousands of concurrent users to emulate a specific workload model based on an agreed transaction rate (or transaction throughput). Achieving this through manual testing is extremely difficult as it involves having multiple testers at our disposal who would be working on client workstation executing different workflows. Also co-ordinating all these testers to do the same thing, bring them in sync and eliminate manual error while capturing the relevant response times readings is virtually impossible.

![Testing Challenges]({{ "/assets/img/testing_issues.png" | absolute_url }})

Fig 2: Perils of using manual testers for Performance testing

Fig 2 above describes how it can difficult it can be when manual testers are used for exercising load on a system. It is self- evident that a Performance test tool is needed to provide the capabilities of load simulation, co-ordinating virtual users, configuring workflows with appropriate transaction rates, monitoring and collecting performance indicator data.

A performance test tool can seamlessly put demand on a system and measures the system behaviour. It does this by generating messages between application components rather than simulating interactions with the user interface. These messages can be stored as scripts and can be generated by recording feature available with the tool. Performance test tools also provide analysis of test results and robust reporting.

One of the big advantages of using Performance Testing tools is the ability to scale out horizontally when additional workload needs to be injected into the system. Most opensource and commercial tools allow for horizontal scalability i.e. addition of new load generation servers into the pool to allow for generation of additional virtual users. Thus using a Performance Testing tool allows for a lot of automation, repeatability, accuracy in measurement of outcomes, consistency in terms of actions including the ability to scale on demand (at-least that works in theory, unless you are constrained by your IT due to lack of availability of infrastructure).

This document will go over the various dimensions or variables that one would consider when choosing a Performance testing tool to match your testing needs.

### What are the different types of Performance Tests one could perform with a Performance Testing tool

There are various different types of Performance Tests that one could perform. Let’s take a few minutes to review the different types of Performance Tests.

* Load Tests
* Soak Tests
* Stress Tests
* Break Tests

The list provided above are some of the most common type of Performance Tests that are executed by SPE (Systems Performance Engineering) professionals. Due to lack of standard terminology you will hear different names or terminology being used, so don’t stress out too much. Let’s quickly take a look at the definition of each of these different types of Performance Tests.

* **Load Testing**: Load Testing are those kind of tests where a given workload (combination of various different business processes scripted into sets of transactions) are injected into the SUT (System Under Test). The objective of a Load Test is to understand the behaviour of the system for the given workload, concurrency, transactional throughput, etc. by capturing the various key performance metrics including end user response times.
* **Stress Testing**: Stress Testing involves subjecting the SUT (System Under Test) to various peaks and troughs of workload i.e. surges in demand and drop in demand, over the expected time interval. The nature of the trough and peak would depend on your workload models which in-turn should be dependent on what business expects to see on the system once it goes live. The objective of Stress Testing is to understand how the system would cope to sudden increases and decreases in workload over short time intervals e.g. start of business when you might have a sudden burst of users logging in or Close of business where you might have batch jobs overlapping with OLTP (Online Transaction Processing Workload).
* **Soak Testing**: The objective of Soak Testing is to understand how the system behaves over an extended period of time. Soak tests are generally run for a normal workload over a large duration of time i.e. 8-10 hours, 1 day, 2 days, etc. The workload used for Soak Tests usually replicates the normal user workload including the expected peaks and troughs in user workload. Soak Testing doesn’t necessarily imply that you would inject peak workload into the system for the entire duration of the test run (unless there was a real world case for that) but rather injection of a real user workload over an extended duration of time to identify memory leaks, management of temporary variables, system stability, etc.
* **Break Testing**: The objective of Break Testing is quite apparent from the name of the test. Break Testing generally aims to understand the breaking point of the SUT (System Under Test). As part of Break Testing one would generally ramp up the workload to a point where the system can’t cope any more. This is generally indicated by the following behaviour i.e. increase in concurrent users being injected by the Performance Testing tool doesn’t translate into an increase of transactional throughput.
We hope these definitions of the various types of Performance tests we will be on the same page with regards to some of the scenarios that these Performance Testing tools (opensource and commercial) will be chosen to execute.

### Does my choice of Performance Tests impact my choice of tools

The impact of your choice of tool on the nature of Performance Test you would like to run are limited but nevertheless do exist. In this section we will take a look how certain limitations with regards to the tool can impact your ability to execute certain type of tests.

As defined earlier the most common types of Performance Tests performed are as follows:

* Load Tests
* Soak Tests
* Stress Tests
* Break Tests

Your choice of a Performance Testing tool impacts your ability to performance tests in the following ways:

* **Load Tests**: Your performance testing tool’s ability to scale and generate the size of your workload i.e. 100s or 1000s of Virtual Users, depends on its ability to scale. Certain tools have scalability limitations which could depend on various factors i.e. type of protocol you have chosen, type of infrastructure you’ve deployed the tool on, etc. While not a big show stopper since most tools scale horizontally you want to be aware of the scalability limitations imposed on your ability to execute Performance Tests.
* **Break Tests**: Your performance testing tool might be able to scale to your existing workload e.g. 1000 users but might have scalability limitations past a certain threshold. This again ties back to the previous point we have made with regards to the scalability limitation of the performance testing tool or in some cases the test rig i.e. a combination of the performance testing tool configuration, environment configuration, storage configuration, network configuration, compute resources available, etc.
* **Soak Tests**: Some of the Performance Testing tools tend to display stability issues when collecting large amounts of performance test data and visualizing it at the same time during extended test runs. The solution in this case is to turn off the visualization of the data while the soak tests are running and wait until the end of the test run to visualize and analyse the resulting performance metrics from across your application landscape. It’s not the best solution but it will allow you to progress with your testing and ensure you don’t lose your test results half way through the performance test run. This in our experience is a bigger issue with some of the open source tools which provide the ability to visualize performance while running the performance test.

In most cases Performance Testing tools allow you to scale the deployment horizontally by throwing in additional compute resources. This however, will only work until a certain point due to the limitations of the central node to keep up with the processing demands of the remote instances. The more mature tools promise good horizontal scalability but experience tells us that scalability is a factor of the configuration you’ve deployed your solution in. Nothing’s infinitely scalable and unless you’ve designed your Performance Testing rig for scalability expect to hit performance issues with your Performance Testing setup.

Experience also tells us that vendor supported tools are to some extent better at horizontal scaling, however make sure you ask simple questions like:

* What’s the recommended configuration for the performance testing controller
* What’s the recommended configuration for the performance testing load injectors
* What’s the scalability limitations (horizontal) for the protocol I’ve chosen

Understanding the deployment architecture of your Performance Testing tool environment will help you identify any potential scalability constraints. Where possible perform a Proof Of Concept to validate the scalability before you make the final investment.

### Dimensions to consider when selecting A Performance Testing Tool

Choosing a Performance Testing tool is an interesting challenge. There are various dimensions you need to evaluate your tool on and while it’s impossible to cover all the dimensions we’ll do our best to provide an overview of some of the most common and relevant ones:

* **Scalability** – As we have discussed earlier scalability of Performance Testing tools is a factor of the protocol you’ve chosen combined with the deployment configuration for your environment. There’s nothing like infinite scalability. Where possible perform a Proof Of Concept to validate scalability of your tool with your vendor before you make the investment.
Protocol support – Protocol support is potentially one of the most important factors you would consider when deciding on a Performance Testing tool. Different vendors focus on different application protocols e.g. http, https, citrix, ftp, ssh, etc., and your choice of tool will depend on the nature of application protocols you would like to make use of. Experience also tells us that going by what the “Documentation” says is not really a safe thing to do. When it comes to complex application protocols like Citrix, SAP GUI, etc. you want to get re-assurances from your vendor that the protocols are supported and also confirm the nature of support by speaking to some of the Performance Testing experts out there. The nature of support for a given application protocol, will vary from one tool to the other making scripting in some tools (For a given protocol) a lot easier than others.
* **Licensing restrictions** – Licensing is another major challenge with most commercial solutions which you need to be well aware of. Commercial tools tend to have stronger protocol support and support for larger number of application protocols but come with licensing restrictions that could impact the way you would like to make use of the solution. Tool licensing in some cases allows or disallows the use of tools by your vendor (assuming you’ve outsourced the application maintenance/support) and in some cases does not allow the Performance Testing tool to be deployed outside a certain geography. Whatever be the nature of limitations, you ought to know about them when investing in the solution.
* **Support for your Workload Model** – Different applications have different combination of workload i.e. OLTP (Online Transaction Processing), Batch, Workflow, Messaging, etc. and your choice of tool will depend on the nature of workload models you would like supported. Most enterprise tools are flexible in the nature of workload you are allowed to design but if there are limitations on the ability to design complex workload models it’s definitely something you would like to know upfront.
* **Vendor support** – Choice of tooling to a great extent in large commercial enterprises is driven by the availability of commercial vendor support. Commercial Performance Testing tool vendors will offer support of various forms which you should definitely evaluate to see if it meets your needs. With regards to open source tools, there are quite a few open commercial platforms built on top of these tools that offer services and support. You should evaluate them to see if these commercial platform built on top of the Open Source solutions meet your enterprise needs.
* **Community support** – Community support is another factor that you should consider when investing in Performance Testing tools. The availability of online forums where you could reach out for support is definitely something worth considering. Experience suggests that depending on vendors too much is definitely not a good option, build capability on the technology to the extent desired (and supported by the IT budget) but also ensure your team is plugged into the relevant industry technical forums to stay abreast of the latest developments, patches, vulnerabilities including functional updates.
* **Availability of skills in the Market Place** – Probably one of the most common dimension that will come to mind when selecting a Performance Testing solution. A simple search of any of the large job sites (local to your country) will give you an idea of the nature of capability available locally. This would differ from region to region so we would definitely recommend doing your homework to understand which way is the market skewed. Un-fortunately the market in most geographies is skewed to some of the enterprise Performance Testing tools. Don’t let that bog you down if you have the budget to build capability on the smaller and lesser known tools but it pays to understand the skills landscape before you go in and commit investment on a certain enterprise Performance Testing platform.
* **Enterprise collaboration** – Support for enterprise integration and use might be a requirement for some large organizations. Standalone Performance Testing tools might cut it when considering standalone projects or one large program, but as soon as you have a large organization spread across multiple geographies wanting to leverage the investment in tools you have to start thinking along the lines of enterprise capability and support from a Performance Test tooling standpoint. The degree to which Performance Testing tools allow enterprise wide use and integration from a single shared/distributed platform is something worth investigating. Again like most other areas the industry leaders in the Performance Test tooling space probably have stronger offerings than those who support one or two application protocols or niche markets. Open Sources tools on the other hand mostly lack support for enterprise use requiring manual co-ordination of testing resourcing or possibly going down the path of siloed investment in platforms for different parts of the enterprise.
* **Integration with Monitoring & Diagnostics tools** – Performance Testing tools are at their best when you are able to integrate them with the monitoring and diagnostics tools that live within the enterprise. The landscape for monitoring and diagnostics tools is so large that it’s quite impossible for every Performance Testing vendor to support every conceivable monitoring and diagnostics solution out there. We would highly recommend doing your homework to understand what your internal landscape of monitoring and diagnostics tools looks like and then confirming support (including the extent of integration) with your tool vendor. Ask relevant question and pilot the integration to convince yourself of the nature of metrics you can pull from the monitoring and diagnostics tools.
* **Adaptability and extendability** – Our applications these days consist of complex in-house and 3rd party components. In some cases the capability of the performance testing tool is limited but you are able to pull in metrics from other solutions using API’s exposed by the vendor of that solution i.e. for purposes of monitoring, extending testing functionality, etc. In such cases having the ability to extend the functionality of your Performance Testing tool to integrate with 3rd party API solutions will definitely help. Again, like most other dimensions we would highly recommend performing a Proof Of Concept to validate the integration before you commit investment to the given platform.
* **Integration with Requirement Management & Defect Management tools** – Most of the enterprise Performance Testing tools offer integration with the industry leading Defect Management and Requirement Management tools. Conversely Performance Testing tool vendors can’t support every commercial defect management platform out there. So do your homework to understand what the level of support is and the effort required to integrate with your enterprise Defect Management platform. Integration with the defect management platform in some of the cases is a pre-requisite to be able to track the test cases and defects that are generated by the Performance Testing tool. While not a major concern from an implementation standpoint it could be a show stopper if not looked at when evaluating the various Performance Testing solutions out there.

### What Are My Options: Open Source & Commercial

There are a few Open Source Performance Testing platform and a number of commercial options. This section does not intend to provide a comprehensive view of all the options out there but does list some of the most relevant ones.

* Commercial
  * NeoLoad – www.neotys.com
  * Load Runner – www.hp.com
  * Keynote – www.keynote.com
  * SOASTA – www.soasta.com
  * Blazemeter – www.blazemeter.com
  * Webload – www.radview.com
* Open Source
  * Gatling – www.gatling.org
  * Jmeter – www.jmeter.org

This list isn't meant to be exhaustive in nature. There's tons of performance testing tools out there and we have included the most common tools used in the industry.

If you have come across other relevant options which are not included in the above list please drop us a note with the relevant details and we would be glad to have them included.

### Protocol Support: What Protocol I Am Going to Need to Record My Scripts In

Performance Testing generally focuses on understanding the scalability and performance limitations of a given system at large workloads. Unlike functional tests where the tester has to simulate one connection, Performance Testing requires the generation of large volumes of concurrent users. Over time as tools have matured vendors have come to a realization that the best way to scale a performance testing tool is to design it such that the tool captures and replays network communications with application level visibility. Let’s quickly look at how a Performance Testing tool works:

* Developer installs the Performance Testing tool (Developer interface) on his desktop
* Developer then manually performs a given transaction
* The Performance Testing tool sniffs the wire to capture all the relevant traffic
* The captured traffic is then presented to the user as a script which can then be enhanced
* The developer designs relevant scripts using that capture, parameterizes and correlates as required (to substitute dynamic content, variables, cookies, etc.)
* The developer tests the scripts and ensures that the script is able to deal with the dynamic variables that the application throws at it

The most optimal way for a Performance Testing tool to scale is to replay the scripts (developed using the procedure above) for a large number of users. With all of this in the background you would now understand the importance of the protocol that the application uses to connect to the client. In case of a web application the protocol would be http/https. In case of SAP it could either be http/https or SAP GUI. In case of streaming application it could be rtmp. Understanding your application protocol and confirming tool support for the given protocol is an essential pre-requisite.

Most performance testing tools out there have support for http/https while some enterprise tools have support for more complex application protocols like Citirix, SAP GUI, SSH, FTP, etc. Vendors tend to license tools based on a combination of various factors and the number of protocol packs is one of those important dimensions. So spend time understanding the protocols your applications use and factor that into your tooling approach.

### What Are the Factors That Affect Tool Licensing Models

This only applies to commercial Performance Testing tools and not to any of the Open Source Performance Testing tools. Here’s a view of some of the factors that vendors take into consideration when pricing Performance Testing tools:

* Protocol Bundle – Protocol bundle refers to the different protocols that the Performance Testing tool will support or allow you to execute Performance Tests in. See the earlier section for an understanding of the importance of protocol support and what protocol support really means.
* Locations of use – Vendors also tend to price tools based on location of use. Some of the leading Performance Testing tools provide the following tiered approach:
  * Local use i.e. for use within a given customer environment within a given city/state
  *  Global use i.e. for use within a customer environment across geographies
  * Global use by 3rd party i.e. for use by the customer’s vendor providing support services
* Number of Concurrent Users – As the name suggests the number of concurrent users licensed limits the maximum number of virtual concurrent users that the tool is able to simulate during a performance test.
* Duration Of Use – Like most other software vendors tend to provide term or perpetual licenses for their solutions.
* Support Required – Vendors also tend to offer different levels of support with different turnaround times or SLA’s for support provided.

Please do keep in mind that not all of the above factors will apply to every vendor and it is also likely that we haven’t included all the dimensions that each vendor takes into consideration. So please take time to understand your vendor’s licensing model and how the various factor’s we’ve discussed affect the licensing costs of the Performance Testing tool you’ve chosen to invest in.

### What Fancy Workload Models Will I Need To Design

One of the other interesting features of Enterprise Performance Testing tool is the ability to create realistic workload models. If you’ve been doing a bit of reading here at Practical Performance Analyst you would have realized that Workload Models are the combination of tasks that the system performs. Workload models include combination of OLTP (Online Transaction Processing), Batch, Workflow and Messaging requests, basically all the different components of the application that consume computational resources. The ability to the tool to create realistic workload models will determine your ability to inject realistic workload into the system.

Enterprise Performance Testing tools are known to offer better support for complex workload models as compared to the Open Source ones. The Open Source tools offer elementary support and in our experience leave a lot to be desired when it comes to generating realistic Workload for purposes of Performance Tests. This doesn’t mean you shouldn’t use Open Source tools, please do but keep in mind the limitations

### What Concurrency Should the Tool Support

Performance Testing requirements will differ from one project to another and the nature of workload (OLTP or Online Transaction Processing, Batch, Messaging, Workflow, etc.) will determine how you go about building your Workload models. The nature of your workload also defines your concurrency requirement e.g.

* For a system being designed to support 1000 seats in a call centre the actual concurrent user base among the 1000 seats might only be 500 (assuming that 50% of the population is active at any point and speaking to customer). This is an unusually high number for concurrency but given the nature of system being designed, the high numbers of concurrent customers does make a lot of sense.

* For a system (integration layer) being designed to integrate with external 3rd party vendor systems the concurrency requirements would be limited to the number of connections the system would initiate and receive at peak.

The concurrency required from a Performance Testing tool is a factor of your peak workload for your given SUT (System Under Test). We would recommend that you do your homework to understand the nature of your Workload and armed with that information you work with your Performance Testing Tool provider to identify a suitable solution.

### What Scalability Considerations Should I Have In Mind

Scalability of your Performance Testing tool is tied closely to the Workload you need to inject into your system for purposes of Performance Test. Most of the Industry Standard Performance Testing tools are known to scale to thousands of Virtual Users (Concurrent Users). With regards to HP’s Load Runner we have seen scalability go past 70,000 to 80,000 Virtual Users (Concurrent Users) using the cloud to generate massive volumes of that workload.

However, the scalability of the underlying Performance Testing infrastructure combined with the scalability of your chosen Performance Testing solution in many ways will limit the maximum number of Virtual Users (Concurrent Users) you are able to connect. We would recommend that you do not take anyone’s word for scalability of the solution but rather validate the Performance and Scalability limitations of your own kit to understand its breaking point. Armed with that information you are better able to make decisions around the nature of Performance Testing engagements you are able to support. You obviously want to avoid situations where your Performance Testing solution i.e. tool, compute infrastructure, storage or network infrastructure, has ventured into its ZNLP (Zone Of Non Linear Performance i.e. >75+% Utilization) leading to increase in queueing, hence increase in overall service times and leading to skewing of your final Performance Testing results.

### Does My Enterprise Need Customer Support

This is a question you have to ask yourself and will be based on various criteria. A lot of the Open Source options out there have limited commercial support available but have a vibrant community of developers and testers who are able to provide support. However, If you are a large organization with distributed teams combined with vary large and complex application portfolios you might definitely have considered going down the commercial tool route. In such a situation you do not have much choice and will most probably be investing in support from the vendor to help troubleshoot and issues that your teams encounter when using the Performance Testing tool.

With regards to commercial support offerings for Open Source Performance Testing solutions, there’s a lot out there and you should definitely do your homework to understand what works best for you.

### How Much Is My Enterprise Willing To Spend i.e. Commercial v/s Open Source tools

What your organization is willing to spend will in a large way influence your tool choice. Performance Testing tools tend to be expensive and the licensing models a bit outdated in some cases. The advent of the cloud has in some ways forced Performance Testing solution providers to revisit their licensing models and adapt them to the cloud. However, most Performance Testing tool providers have a long way to go with regards to simplifying their licensing model. Your IT budget will dictate what you can spend which will drive your ability to invest in one of the Industry Standard Performance Testing solutions out there.

Whether you go Open Source or Commercial, you should definitely do your due diligence to understand the nature of your organizations requirement for tooling which to a large extent will be driven by the type of application portfolios you have (think application protocols, etc.) combined with the nature of workload these applications expect to receive in production. Armed with some of that information you can make a more educated guess about the fit of Open Source or Commercial Solutions to your given requirement.

### How Much of Development Effort Are You Willing To Spend on Your Scripts (i.e. Commercial v/s Open Source tools)

While I am inclined to say Commercial tools are generally more mature across the board its horses for courses i.e. your choice of a Performance Testing solution should be driven by your application portfolios (application protocol) and nature of the workload you need to generate for purposes of Performance Test. Keep in mind that generally Open Source tools offer lower scalability (when compared to some of the Industry Standard Performance Testing solutions) and also offer limited support for complex scripting tasks i.e. parameterization, correlation, etc.

Open Source solutions to some extent might also require a patch work of various other open source or commercial plugins to support your complex workload requirements. So be aware of what you are getting into. Open Source is great for Performance Testing when you have a relatively simple workload, do not have fancy workload models i.e. mix of OLTP, Messaging, Workflows, etc., do not have many fancy protocols you are dealing with i.e. Siebel, Citrix, etc. and have low concurrency numbers. Open Source Performance Testing tools like Jmeter, etc. have been around for a while, offer simple workload modelling capability, scalability issues when you go past a few thousand Virtual Users (Concurrent Users) unless you’ve tuned the system really well, have very limited reporting, analysis capability and very limited support for anything other than HTTP/HTTPS application protocols.

The intention here is not to down play the importance or capability of Open Source Performance Testing solutions but rather to stress on the fact that the development, maintenance and operational support for Open Sources tends to be a lot higher than most commercial Performance Testing solutions. If you are a medium to large organization with moderately complex to complex workload, a large application portfolio with an assortment of protocols that you need to support and high concurrency numbers (thousands or hundreds of thousands) you should definitely consider Commercial Tooling options and work with your vendors on evaluating them for your particular needs.

### Am I Expecting to have Automated Correlation, Parameterization & Analysis Capabilities Built into the Tool

Parameterization and Correlation are important activities that every Performance Testing Engineer has to perform when writing most scripts. Let’s look at the definitions of these two terms in short:

* **Parameterization**: The ability to identify and place variables for key elements in the script so that appropriate values can be provided for every iteration e.g. Let’s assume you have a registered user base of 100 users and a concurrent user base of 10 real users, one of the most important parameters would be your login credentials. As part of the scripting process you would need to parameterize your login credentials and provide the Performance Testing script details for 100 users so that it can iterate through the various user credentials during the Performance Test.
* **Correlation**: Correlation is slightly different from Parameterization but goes along similar lines. Correlation refers to identifying variables in the script where you pick up data sent by the server that identifies a unique transaction and replay those variables as part of the response the server is expecting. For e.g. Most web applications will generate a session ID and most application servers would expect the user’s session (browser) to return the session ID as part of the response. This allows the Application Server to track the session and correlate the request from a user to existing sessions which it maintains within an internal session table to ensure it is sending relevant data in continuation of the customer’s request.
* **Analysis**: Ability of the Performance Testing solution to consolidate the data generated from the Performance Test from across the entire Performance Testing environment and provide a variety of detailed and summary views of all the relevant system performance metrics.

Not every project or enterprise requires automated Parameterization and Correlation. Most Industry Standard Performance Testing tools offer automated Parameterization and Correlation capability. However while the capability does exist it’s not going to pick up 100 of all the variables across the script requiring Performance Testing Engineers to manually Parameterize and Correlated the non-obvious ones. With Open Source Performance Testing tool, you will mostly find no automated Parameterization or Correlation capability and in some cases very limited capability. If this is a requirement for your organization or team then it should drive your decisions around the nature of Performance Testing tool you choose to invest in.

### Is this a Silo i.e. Project specific or an Enterprise Investment

One of the important aspects to consider when identifying a suitable Performance Testing tool is if you intend to use the Performance Testing solution in a silo i.e. a single project or program, or if you intend to use the solution across multiple projects across the enterprise. Some of the Industry Standard Performance Testing tools offer the following capability:

* Automate Scheduling of Performance Tests
* Integration with other commercial Defect Management Solutions
* Integration with other commercial Requirement Management Solutions
* Collaboration across multiple teams
* Centralized management of all Performance Testing licenses, assets and resources
* Distributed Execution, Reporting and Analysis capability
*
Open Source Performance Testing tools offer almost none of the above capability that most enterprises would expect. Some of the commercial ones also are limited in what they can offer so make it a point to understand the needs of your project, program and organization. Armed with an understanding of how the Performance Testing tool is going to be used across the enterprise you can make a more intelligent decision around the nature of Performance Testing tools you invest in.

Open Source Performance Testing tools are also quite limited when it comes to automate Analysis of Performance Testing results and the ability to layer Infrastructure Performance & Network Performance metrics on top of the Application Performance metrics it has collected. Commercial Tools on the other hand do off some integration with monitoring and diagnostics tools being able to layer the relevant system performance metrics on top of the Application Performance metrics to provide a holistic view of the overall system performance.

### What Deployment Architectures are supported

Your choice of a Performance Testing tool will also depend to a great deal on the application architecture you need to support, the application protocols (http, https, citrix, etc.) you need to support combined with the deployment architecture you are looking to invest in i.e. SaaS based tools, on premise tools, etc. Here is where some of the Open Source tools might shine over the Commercial Performance Testing offerings.

Most of the Open Source tools i.e. Jmeter, Gatling, etc. being the product of the Open Source community allow for easy integration with Infrastructure Automation solutions allowing you to automate build and scale out of Performance Testing infrastructure on the cloud. Whether you are using Amazon Web Services, Azure or Rackspace you should be able to leverage open source tools to automate build and scale out of the Performance Testing solution on the cloud. Commercial tools on the other hand are limited on the amount of automated integration and scale out capability they provide. As an end user you should still be able to use open source tools to automate build and scale out of the environments but automation of integration of these Commercial Performance Testing tools is limited and should be investigated on a case by case basis.

### Does The Tool Need to Integrate with Monitoring & Diagnostics solutions

Use of Diagnostics and Performance Monitoring tools on various Performance Testing projects is quite becoming the norm. As you would know Diagnostics tools offers the Performance Engineer the ability to dive deep into the Java Virtual Machine or the .Net Virtual Machine (CLR) and identify code paths that are potential bottlenecks. Diagnostics tools allow Performance Engineers to visualize the code execution paths across the entire stream of downstream systems (Assuming they are all instrumented) drastically reducing the time to identify and address a bottleneck across the system.

Performance Monitoring tools on the other hand provide Performance Engineers the high level diagnostics they require to understand how each of the components across the entire system is performing. This generally would include Performance Metrics across the application, infrastructure and network landscape.

From a Performance Testing standpoint you would definitely like to have the ability to integrate with the Diagnostics and Performance Monitoring tools that your organization owns. Different Performance Testing tools provide different API integration capability and also have licensing models that allow or disallow API integration with other tools i.e. Diagnostics and Monitoring solutions. So be sure to check with your Performance Testing tool vendor if they have support for the relevant Diagnostics and Monitoring solutions you have in house and what is the type of licensing required to be able to build integrations with those products.

### What Are the Training Options Available For the Tool You Are Considering

Whether you are investing in a Commercial or an Open Source solutions having access to relevant training is really important. Some of the leading Open Source tools have a vibrant user community and also large number of vendors offering commercial training offerings. With regards to commercial Performance Testing tools it’s quite a different story. You should definitely do your homework to understand –

* What training options does your vendor provide
* What free e-learning modules does your vendor provide
* What are the costs of the relevant training modules
* Are there other partners out there who offer such training modules

Training staff and creating relevant capability on the Performance Testing solution within the enterprise is highly essential. You want to make sure that the enterprise Performance Testing solution you are investing in can be supported through various commercial training offerings available at an affordable price.

### What Are the License Costs

Licensing models differ from one vendor to the other and costs for tooling differ from one vendor to the other. Industry Standard Performance Testing tools generally tend to be expensive and it’s important that you factor the costs into your proposal. Do your homework on the following areas before you begin the discussions around commercials with your vendor –

* What are the different locations I intend to use the tools from
* What is the total user concurrency I am looking at for all the projects who intend to use the tool
* What are the different protocols (http, SAP GUI, etc.) that our projects require
* What is the split of user concurrency across these various protocols
* What is the duration for which I need these protocol packs for each of my projects

Armed with the above information you can now have a more meaningful conversation with your tooling vendor.

### How Strong Is the Vendor/Community Ecosystem & Vendor Support

Vendor support and community/ ecosystem support is one of the most important driving factors with regards to choice of the relevant Performance Testing solution. Based on our experience we would suggest that you not assume that the large Industry Standard Performance Testing tool vendors have a strong support ecosystem. Sometimes it’s the middle tier or the smaller organizations who have a stronger support ecosystem and tend to do a better job.

However, these are just guidelines based on our experiences and you should do your homework well with regards to the nature of support available from your partner/vendor. One of the other options would be to work with a local channels partner (of the Performance Testing solution you have chosen) who has experience selling and delivering the tools across your geography. This will ensure that you are able to tap into the local support structure and bring on the relevant skills when you need to address burning technical issues.

### Is The Tool Devops friendly and Does It Integrate with my CI/CD Pipeline 

Devops, Continuous Integration, etc. are some of the new paradigms that have recently infiltrated the technology world with the objective of streamlining and optimizing the way technology is building and delivered. While we do not intend to go delve into Devops, CI, CD concepts, it would help that you ask the relevant questions of your vendors to understand the nature of automation and support available within the Performance Testing solution for your internal Devops processes.

### Conclusion

This document aimed to explore the various dimensions you should be considered when evaluating Performance Testing solutions for your enterprise. We have tried to make this document as comprehensive as practically feasible but understand that it’s impossible to cover every perceivable scenario and apologize for not being able to do so. We hope this document has been useful in helping you understand the various relevant dimensions and ask the relevant questions of your vendors helping you narrow down your relevant options. Please do drop us a note with your thoughts, inputs, comments and feedback to feedback at practical performance analyst dot com.

