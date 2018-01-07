---
layout: post
title: Do You Have What It Takes
tags: [Systems Performance Engineering]
author: tangowhisky37
---

**The conundrum** - Numerous times in my career I have encountered situations where clients demand engineering skills but are reluctant to pay for those niche skills. Clients expect to pay rates for a skilled Performance Testing resource but instead expect a seasoned Performance Engineering resource and it does take a while to communicate to the client the subtle difference between the two including the outcomes each of them are skilled to deliver. Smart clients who understand the difference in value proposition consider investing in the niche engineering skills they might require to get the job done.

*This article was originally published at Practical Performance Analyst (older website) on the 7th of November 2016.*

Having said that I have personally also stumbled across a fair few experienced professional Performance Testing and APM (Application Performance Management) resources who aspire to move into the engineering space but are unable to find the support to help them figure out what is required to get there. This article is for them and for everyone out there who might have found themselves confused at some point with regards to the nature of work done by the two including how might one build the skills to both be able to look at the forest for the trees including the ability to look at the trees in detail i.e. macro level view or a micro level view.

**Diving into the detail** - So let's start out by having a look at what Merriam Webster has to say about definition of the word "engineer". Merriam Webster defines an engineer as -

> A person who has scientific training and who designs and builds complicated products, machines, systems, or structures: a person who specializes in a branch of engineering. Most of us would agree with the above definition of an engineer. 

A testing professional (within the Software Engineering space) on the other hand could be described as an individual who specializes in testing or validating the capability being delivered. Testing from a Software Engineering standpoint can be broadly classified into Functional and Non Functional testing both of which are really vast topics and not areas that we are able to dig into with any detail in this piece. For more details on Non Functional testing and Non Functional Requirements please visit the SPE HowTo section at Practical Performance Analyst [Link](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/spe_howtos/).

Functional testing as you would might already know, involves use of various processes, tools, capability with the objective of validating the functionality or capability being delivered by the solution while Non Functional testing pertains to use of processes, tools, capability with the objective of validation of the various Non Functional attributes of the system being delivered. Some of the relevant Non Functional attributes could include â€“

* Availability
* Reliability
* Scalability
* Security
* Performance
* Usability
* Recoverability

Clearly just looking at the above definitions you would agree that engineering is a very different outcome to be delivered as compared to those being delivered by a Functional or Non Functional testing. An important point worth noting here is that Performance Engineering is a discipline within the Software Engineering space and encompasses many different activities across the delivery life cycle (agile, waterfall, etc.). Key point to note though is that Performance Testing is one of the critical activities but not the only activity within the Performance Engineering space. To dig deeper into the Performance Engineering Life cycle and understand it's various components please head off to [Link](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/spe_fundamentals/).

**Let's now look at Performance Testing in a bit more depth** - So finally, let's come to the definition of Performance Testing. Performance Testing as an activity within the Performance Engineering lifecycle (part of the Software Engineering cycle) aims at delivering an outcome which consists of validating the key Non Functional attributes of the system related to scalability, performance. Some of the types of testing that make up Performance Testing include â€“

* Load Testing
* Stress Testing
* Volume Testing
* Break Testing
* Soak Testing

To learn more about the fundamentals of Performance Testing please visit - [Link](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/spe_fundamentals/). On a Performance Testing project a skilled performance testing resource would ideally go through the following steps â€“

* Identify the key Non Functional attributes of the system
* Design the system workload
* Identify a suitable performance testing tool including APM (Application Performance Monitoring / Management) tool
* Deploy the tools
* Record the scripts for key transactions part of the workload
* Design the scenarios and inject the workload in the system
* Work with the engineering resources to identify areas of optimization

Performance testing usually requires design, build, execution of load/stress/volume/break tests and reporting of system performance metrics like transaction response time, concurrent user loads supported, server throughput, etc. combined with key infrastructure and software performance metrics e.g. browser performance, method level performance, server resource utilizations, buffer pool utilization, cache utilization, etc. A combination of the end user experience metrics combined with the relevant software and hardware metrics is key to understanding the overall system performance and is usually what a performance testing outcome aims to capture or deliver.

Based on what we have just covered you would expect a Performance Testing professional to be able to design, build and execute performance tests. Assuming a simple 3 tier architecture, the performance testing outcomes would include performance of individual tiers - web server, application server & DB server, client-side / browser performance, network performance, server hardware performance, etc. The key different being a good performance testing resource will execute tests, capture the relevant application, end user experience and infrastructure performance metrics so that they can be reported. A strong performance engineering resource however will take things to the next level. Read on to learn more.

**Let's now look at Performance Engineering in a bit more depth** - Let's start with the definition for Performance Engineering. Systems Performance Engineering (Which is what we prefer to call it) is a discipline within Systems Engineering that involves systematic practices, techniques & activities during each phase of Software development life cycle (SDLC) to meet performance requirements. Systems Performance Engineering strives to build performance standards by focusing on the architecture, design & implementation choices. To learn more about Systems Performance Engineering and the associated fundamentals please visit [Link](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/spe_fundamentals/).

Systems Performance Engineering stresses the need to view Performance proactively throughout the software development phases right from the requirements phase until the operational phase. In this proactive mode -

* A Performance Engineer is involved right from the initial requirements gathering phase ensuring that the relevant Non Functional Attributes are defined (has direct linkage to the expected business outcomes) appropriately,
* At the design phase where the Performance Engineer works with the design team on selecting sensible design patterns for performance/scalability (based on the agreed Non Functional Requirements)
* At the Performance Testing phase where the Performance Engineer is responsible for working with his team of Performance testers to put together the approach
* Then execute based on the agreed approach
* Finally onto the operational phase where the Performance Engineer is responsible for putting in place a relevant monitoring/management approach which could involve use of analytics solutions (Splunk) combined with APM (Application Performance Management) solutions to measure and report on system performance.

In contrast when looked at from a reactive standpoint, when a system is tested at the end of the development phase and various performance, scalability defects have been identified i.e. the system does not meet the non-functional requirements related to response time SLAs, user scalability levels, etc., then a Performance Engineer could be brought into to understand the metrics reported by the underlying system or work with the existing development/performance testing resources to understand the work done before diving into the system performance issues using his/her diagnostics tools to identify the root cause of the issues being seen.

The Performance Engineer can then recommend executing specific tests and instrumenting the system to capture relevant performance metrics so that he/she is able to dive into the code with the objective of isolating the bottleneck. In this case, depending upon the bottleneck reported, the Performance Engineer could choose to bring on-board specific performance SMEs like DB architect, application server specialist e.g. Websphere specialist, Oracle middleware specialist, Mulesoft integration engineer, Network Engineer, etc. so that they might be involved in analysis of the performance issue.

There are no hard and fast rules with regards to what a Performance Engineer or a Performance Testing engineer could or could not, should or should not do. These are just our personal observations based on years of experience. It has been my personal experience that one does not just turn into a strong Performance Engineer, it generally takes years of developing one's skills in the Performance Testing or Performance Diagnostics space before they decide it's time to start picking up additional skills across the other areas of the delivery cycle. This also tends to happen when individual or professional has gained the ability to see both the forest and the individual trees within the forest as compared to just the forest for the trees.

**What might be a career path for Performance Testers aspiring to become strong Performance Engineers** - Like we have mentioned before there is no hard and fast rule with regards to the path one might consider taking to gaining the skills to become a strong Performance Engineer. What we have touched upon briefly in the previous sections including what weâ€™ve covered in this section should be seen as one possible approach to building the skills required to become a strong Performance Engineer.

Most professionals are introduced to the discipline of Performance Engineering through aspects of Performance Testing or Application Performance Management (APM). Again, there is no hard and fast rule here and your story could very well be something really different. Letâ€™s consider a scenario where you are a Performance Testing professional. As a Performance Testing professional as you have gained varied experience (5-6 years) across projects of different complexities, you have probably built a strong understanding of the processes, tooling, capability, skills, etc., understand how Performance Testing fits in within the larger discipline of Performance Engineering and most importantly appreciate the value it can deliver. Or you could be an Application Performance Management (APM) engineer with a strong understanding of the processes, tools, capability required to deliver APM projects and with 5-6 years of experience under your belt you are now looking to expand your horizons.

In either of these cases you are an experienced professional who has built credible experience across projects of various different complexities, are a master of the discipline (i.e. Performance Testing or APM or Capacity Management or Performance Modelling) you are in, have understood the value that Performance Engineering delivers and are keen to take a broader view of the world.

Aspiring Performance Engineers are usually not specific domain or technology experts but rather they have good understanding of the end to end Performance Engineering life cycle and are able to leverage their depth of technical knowledge to manage Non Functional attributes of the system from requirements gathering until go-live. I have tried to put together a summary of the various skills a Performance Engineering might consider building. Please note that this is not meant to be an exhaustive list but rather a guide of some of the areas someone intending to build a performance engineering career might consider focusing on for the longer term - 

* Strong understanding of the end to end Performance Engineering cycle
* Is a domain expert in at-least one or two areas across the Performance Engineering life cycle i.e. Performance Testing, APM, Capacity Management, etc.
* Possesses good experience in reviewing system architecture / deployment architectures with the ability to work with architects on making recommendations and designing for performance
* Ability to work with customers to understand the overall business requirements, translate them to sensible Non Functional Requirements and then put together a sensible Performance Engineering approach which covers relevant aspects of performance across the delivery cycle.
* An inquisitive mentality, an ingrained sense of inquisitiveness, always questioning the data to be able to get to the root cause of the issue at hand.
* Understanding of the tooling used to deliver the various outcomes across the Performance Engineering cycle i.e. LoadRunner, Jmeter, NeoLoad, AppDynamics, New Relic, etc.
* Experience using monitoring and diagnostic tools to understand system performance. Ability to use the data generated from these tools to dive deeper into the system performance issues and then work closely with the build/development teams on addressing the performance challenges across the relevant systems.
* Experience in analysing the application traffic patterns using tools like Omniture, DeepLogAnalyzer, etc.
* Experience in performance monitoring tools & APM tools like Perfmon, HP Sitescope, CA Introscope, Dynatrace, AppDynamics, etc.
* Good experience in using profiling tools like Jprofiler, Jprobe,Jconsole, VisualVM, HP Diagnostics, etc, including GC / JVM analysis tools & heap/thread dump analysis tools.
* Experience in DB profiling tools like Statspack / AWR / SQL profiler,etc.
* Experience in front end web performance analysis using Yslow, WebPageTest, Ajax Dynatrace, PageSpeed, etc.
* Experience in performance prediction / modelling analysis during early SDLC phases.
* Experience in Capacity planning/sizing through Queuing Theory principles & tools like TeamQuest, Metron Athene, etc.

**Conclusion** - The set of skill sets we have listed above is not definite but rather a microcosm of what you might consider as skills required to become a strong Performance Engineer. As we have mentioned before there is no single path to becoming a good Performance Engineer and each of you with your unique background and unique story will have your own way to getting there. Also, every Performance Engineer might not have skills across all technologies. Based on their practical experience & technical exposure, though they usually tend to have knowledge across a few different technology stacks. However, good Performance Engineers are technology stack and platform agnostic i.e. they carry a very strong work ethic, understand the tools, processes, capability required to deliver outcomes across each of the areas and are able to apply that understand to any performance related challenge that might come their way.

**Authors** -  This article was authored by **Ramya Ramalinga Moorthy**. **Ramya** ([LinkedIn](https://in.linkedin.com/in/ramyamoorthy)) is a Performance Test Architect with over 13 years of experience on Performance Testing & Systems Performance Engineering. She has great passion for learning & experimenting new things. In her current role, Ramya works closely with clients around the world providing them consulting services focused on Performance Engineering, Non Functional Requirements Modelling, Performance Modelling & Capacity Planning. Ramya is passionate about training & mentoring budding Systems Performance Engineers. Her key areas of interest includes Workload Modelling, Performance Modelling & Capacity planning. She has authored & presented several papers related to Performance Engineering in International conferences. And not the least, proud mother of two little princesses. Please additional details on the consulting services Ramya provides please see &#8211; [EliteSouls.Â ](http://elitesouls.in/) Alternatively you can reach her at info@elitesouls.in.

This article was edited by **Trevor Warren**. Trevor Warren is passionate about challenging the status-quo and finding reasons to innovate. Over the past 16 years he has been delivering complex systems, has worked with very large clients across the world and constantly is looking for opportunities to bring about change. Trevor constantly strives to combine his passion for delivering outcomes with his ability to build long lasting professional relationships. You can learn more about the work he does at [LinkedIn](https://au.linkedin.com/in/trevorwarren). You can download a copy of his CV at [VisualCV](https://www.visualcv.com/tangowhisky37). Visit the [Github](https://github.com/tangowhisky37) page for details of the projects he’s been hacking with off late.

Please drop us a note at feedback at practical performance analyst dot com or using the Discuss Chat box at the bottom of this page to engage with the author, ask questions and share your perspective. We are keen to hear from you.

