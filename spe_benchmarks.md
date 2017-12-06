---
layout: pagelayout
title: SPE Benchmarks
menu: true
order: 15
---

### Introduction

Most of us rely on systems of one form of the other to perform our daily routine tasks. Say for example -

* Maintaining details of our regular customers, managing their billing details, dealing with customer queries, assigning of support tickets, etc. is best dealt with a system called a CRM system which some of might be conversant with
* Or a Human Performance Management system which your organization uses to track the Objectives, Progress and Achievements of all it&#8217;s employees so that the outcomes could be tied closely to promotions or the employees remuneration package, etc.

We all deal with systems big and small in our daily lives. It is through the science of SPE or Systems Performance Engineering that Engineers meticulously engineer Performance, Scalability, Reliability, Availability into these system which most of us take for granted. Whatever name you might want to call it i.e. Web Operations & Performance, Front End Performance, Agile Performance Testing, etc. you are dealing with aspects of SPE across the Development & Support Life Cycle. Yes, i know it might sound a lot cooler to say &#8220;Web Operations & Performance&#8221; as compared to SPE (Systems Performance Engineering) but the bottom line is we are still dealing with Engineering of Performance into the system.

Remember the key word here is the **System** and the reference to SPE as Systems Performance Engineering not just Software Performance Engineering.

> _Systems Performance Engineering or SPE defines a set of tasks, roles, responsibilities, deliverables and outcomes at each phase of the system development and support life cycle with the objective of ensuring that the delivery systems meets the documented or agreed Non Functional Requirements_.

So, having defined what SPE means lets dive into benchmarks and the relevance of benchmarks from an SPE standpoint.

### What are Benchmarks 

Benchmark is a standard or a point of reference against which things can be measured. Technically speaking we are all impacted by benchmarks and their accuracy in one way or the other. Let's take for example measurement of the following items:

* Measurement of a litre of petrol
* Measurement of a kilo of grains
* Measurement of 10 ounces of sugar

We expect to be given the same amount (in terms of weight or volume) for each of the above items for relatively the same price irrespective of which retail outlet we purchase them from. The location of the retail outlet, it's height above sea level, the political climate in the country or the weather for the day should not in anyway impact the amount of produce we have procured or paid for. We rarely stop to think the impact of standards or benchmarks in our lives but benchmarks or standards impact almost every part of our life. A centimeter measured in the Cayman Islands is the same as a centimeter measured in the Papa New Guinea. It is such universally accepted global standards for the measurement of produce, that makes business seamless across national and international borders.

Similarly, in the computing world benchmarks exist to allow customers to compare different aspect of the hardware and software that are designed and delivered by manufacturers. Benchmarks are a way customers can validate the claims that are made by manufacturers on what their hardware and software can deliver. Manufacturers put a lot of effort into benchmarks and go to great lengths to prove that the systems they have designed and delivered are the best out performing a large part of the competition. As customers you are called upon to analyze the numbers presented along with details of the system configuration and treat the results with care. Remember benchmarks are controlled experiments and not real world interactions with real world customers.

### So Why do we need Benchmarks

There are various reasons why the industry has agreed for the need for benchmarks. Some of them are as follows:

* To be able to compare the performance of the end system i.e. hardware, software and configuration provided by different vendors
* To be able to make choices on the nature of system specifications one might invest in depending on the need
* To be able to understand the scalability and performance limitations of a given system
* To be able to plan and budget for expenditure for a given set of systems that an organization might be needing to invest in
* To understand the ability of the vendor to meet the organizations transaction processing needs from a performance standpoint

Benchmarks in short offer customers the opportunity to compare different systems i.e. Hardware, Software & Configuration, against each other to understand the Performance, Scalability, Reliability, Availability it can deliver and if those attributes meet the needs of the organization.

### What are some of the Industry Benchmarks which matter

Here are a few industry standards out there that matter when it comes to benchmarking standards. Here are the organizations and the websites which you should consider:

* TPC or Transaction Processing Council &#8211; <a href="http://www.tpc.org" target="_blank">TPC.org</a>
* SPEC or Standard Processing Evaluation Corporation &#8211; <a href="http://www.spec.org" target="_blank">SPEC.org</a>
* RPE2 by Gartner (Previously Ideas International) &#8211; <a href="http://www.gartner.com/technology/research/RPE2-methodology.jsp" target="_blank">Gartner RPE2</a>
* SAPS by SAP as part of the SAP Standard Application Benchmark &#8211; <a href="http://global.sap.com/campaigns/benchmark/appbm_overview.epx" target="_blank">SAP Benchmarking</a>

Each of the above organizations offer different types of benchmarking standards, each of which apply to the various types of systems out there. For example lets consider the following benchmarks from SPEC and TPC &#8211;

* **SPECjEnterprise2010** from SPEC which focuses on Java Client &#8211; Application Server performance
* **TPC VMS** which focuses on performance metrics for virtualized databases

For details on additional benchmarks please refer to the TPC, SPEC, RPE or SAP websites.

No two benchmarks are the same and each benchmark is defined for a different audience. TPC and SPEC are two of the world leading Not For Profit organizations which design the standards for these benchmarks adopted by different commercial organizations from all around the world. TPC and SPEC work closely with commercial organizations from all around the world on designing their benchmarks and keep revising them to make sure they are relevant.

RPE and SAPS on the other hand are owned by commercial entities. RPE2 was introduced by IDEAS International (Australia) which was eventually bought over by Gartner while SAPS is part of the SAP Application Standard Benchmarks owned and published by SAP. Details on both RPE2 and SAP are hard to find unless you have signed up to an NDA or are a Gartner or SAP, partner or potential client.

### How should we be using these Benchmarks

Benchmarks are highly useful to those who deal with Performance, Reliability, Scalability and Availability of systems on a daily basis. Benchmarking standards and benchmarking results allow Performance Engineers to perform some of the following tasks:

* Compare the performance characteristics of any two systems
* Understand the Cost v/s Performance metrics for any two systems
* Understand the potential breaking point for any two systems
* Make design decisions that could be made based on scalability limitations of the systems

Based on the outcome of a benchmark or using benchmark results Performance Engineers might be expected to :

* Design and document High Level Capacity Plans for a given project requirement
* Provide a Bill Of Material (BoM) for a given project to support a given product implementation
* Provide review comments on the Performance/Reliability/Scalability characteristics of a system being proposed by a vendor
* Provide recommendations on consolidation of compute and storage infrastructure
* Provide recommendations on replacement of compute and storage infrastructure

Benchmarks are useful information when interpreted in the right manner. You have to view benchmarking results provided by vendors with care.

### What should one be careful of when using Benchmarking results

Benchmarks as one would expect is a designed artifact executed by a vendor to prove a point. One should keep the following points in mind when reviewing publicly available benchmarkeing numbers:

* Benchmarks are designed within a controlled environments mostly using clean data
* Benchmarks are executed within controlled environments using relatively clean data
* Systems being benchmarked are engineered, specked and configured with the best or largest configurations out there
* Systems being benchmarked are tweaked by experts from the manufacturer who have inside knowledge on how these systems work and are able to bring the best out from these systems
* Benchmarks are executed within constraints that are controllable and do not necessarily replicate the sudden peak and trough of workloads that one would see in a real production environment
* It is highly unlikely that you will subscribe to the same configuration from the same vendor when designing the BoM (Bill Of Material). So treat the Benchmarks as a sense of direction rather than absolutely truth.
* Vendors benchmark servers against different standards i.e. TPC, SPEC, SAPS, etc. as a result the numbers might not be directly comparable
* The open benchmarks i.e. TPC, SPEC, SAPS, etc. do not have published routines or algorithms that allow numbers (results) for a given benchmark (for a given server, configuration, etc.) to be interpreted through the lenses of another benchmark i.e. view TPC-C as SPECS
* RPE2 is the only non-vendor benchmark which we have come across which might go a long way in providing end customers a more holistic view of system performance by allowing comparison against different benchmarking standards

With all the caveats above you are probably wondering if Manufacturers design the benchmark outcomes to mislead. However, that is really not the case. It is just that the way benchmarks are designed do not allow for direct translation of performance metrics into a real world production environment. So be careful with how you use those benchmarking results and compare the numbers with care.

### How do I learn more about these Benchmarks

Learning more about any of these benchmarks is easy. Visit the links provided below to understand what each of the organizations offer and what benchmarks they provide. The specifications and details for RPE2 used to be a lot more openly available until Gartner purchased Ideas International (Owner of the RPE2 benchmark). However details for the various TPC and SPEC benchmarks are available for everyone to see.

* [TPC](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_benchmarks/TPC_Benchmarks/) 
* [SPEC](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_benchmarks/SPEC_Benchmarks/) 
* [RPE2](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_benchmarks/RPE2_Benchmarks/) 
* [SAPS](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_benchmarks/SAP_Benchmarks/) 
* [Miscelleanous](https://tangowhisky37.github.io/PracticalPerformanceAnalyst/pages/spe_benchmarks/MISC_Benchmarks/) 

The information provided here at SPE Benchmarks is meant to get you started with the world of benchmarking groups/platforms and the various types of benchmarks each of them run. For currency of a given benchmark and updates specifications/results please visit the relevant vendor website. 
