---
layout: pagelayout
title: Performance Engineering 101
---

This section will delve into the various aspects of Performance Requirements Analysis as seen from the eyes of the Practical Performance Analyst (some one like yourself). The sections will cover the following topics –

* What is Performance Requirements Analysis
* Why is Performance Requirements Analysis Important
* Activities involved in Performance Requirements Analysis
* Challenges involved in Performance Requirements Analysis
* Going about the Performance Requirements Analysis Process
* Deliverables of the Performance Requirements Analysis process
* Resources on Performance Requirements Analysis

### What is Performance Requirements Analysis

Performance Requirements Analysis is a set of activities performed during the requirements gathering phase of a program to identify the Performance Engineering related objectives for the solution being delivered. These objectives are also called the Non Functional Requirements of the solution. From a Performance Requirements Analysis perspective your Non Functional Requirements would address the following aspects of the solution.

* Scalability Requirements (Peak transactional workload, Peak User Concurrency, etc)
* Availability Requirements (System Availability or up-time. Eg. 99.9999% up-time)
* Reliability and Fail over Requirements (Level of redundancy built into the solution from both an application and infrastructure perspective)
* Performance Requirements (Expected response times, expected parallelism, expected run times, etc)

It is essential to document these Non Functional Requirements so that all the relevant stake holders i.e. application architects, applications designers, business sponsors, developers, testers, production support have an very clear understanding of the performance requirements of the solution being designed and delivered. This is essentially performed at the start of the program by engaging with the relevant stake holders (mentioned above) and documenting all the important facets of performance that are relevant to the solution. Documenting your Non Functional Requirements also gives you, the Practical Performance Analyst the opportunity to set expectations and manage them early on in the development cycle.

As a practicing Practical Performance Analyst you should also use this as an opportunity to get all your stake holders on the same page and agree on all the different aspects of Performance Engineering that are relevant and need to be addressed across the Software Development Life Cycle. The Performance Requirements Analysis phase sets the stage for rest of the Performance Engineering activities that need to be performed across the Software Development Life Cycle. As the Practical Performance Analyst this is a wonderful opportunity for you to socialize your plans and put in the relevant requests for tools, resources, licenses, infrastructure, etc you would need to meet the defined Non Functional Requirements.

### Why is Performance Requirements Analysis Important

Performance Requirements Analysis is the first phase in the Performance Engineering Life Cycle and there are quite a few reasons why we think Performance Requirements Analysis is important and still very relevant in this age of virtualization and cloud computing. A list of reasons are provided below:

* **Determine Non Functional Requirements** – The Performance Requirements Analysis phase can be considered to be the most important phase of the program but unfortunately most organizations or projects don’t have the wherewithal or capability required to ask the right questions and gather the right requirements. Without proper Non Functional Requirements you will have no Performance related objectives, without objectives you can’t set strict goals and without goals there is no measurement possible. Thus it’s important that clients and projects understand the need of bringing on capable Performance Engineering resources early on in the development life cycle of a project to document the Non Functional Requirements and set the stage for the activities that need to be performed on the program.
* **Set Performance Targets for Developers** – As a Practical Performance Analyst, once you have documented your Non Functional Requirements you now are able to set Performance Targets for each of your development teams for the relevant application components across the different application tiers. You should use this as an opportunity to go deep into the design, identify potential application bottlenecks and set stringent Performance Targets for the development teams across the different application components and tiers. These targets would be single user Performance Targets which needs to be defined with some thought. The reason why we suggest Single user performance targets is because at the development stage developers have little idea of what the cumulative performance of the system would be for large number of concurrent users and the only method available to them is to unit performance test their code at the development stage.
* **Validate Architectural Options** – At the Performance Requirements Analysis stage you have the option to review application designs and provide relevant input from a Performance Engineering standpoint given a strong understanding of the project’s goals. The Performance Requirements Analysis stage is the best opportunity for you as a Practical Performance Analyst to dig deeper into the patterns, designs, architecture being recommended and identify potential challenges with the solution. Build good relationships with the customers, your different team leads and most importantly get their buy in. Once your customer and team leads understand your vision, your objectives, your goals and your plan they will understand the reason why you pushing for stringent Non Functional Requirements for critical aspects of the application.
* **Determine Infrastructure Capacity Required** – As a Practical Performance Analyst you have the opportunity to review the Non Functional Requirements and combined with an understanding of the application design you should be working with the vendor and customer to recommend or in some cases validate the underlying Infrastructure requirements. Most vendors of COTS (Commercial Off The Shelf Solution) recommend infrastructure based on a customers Non Functional Requirements for a given workload. The Performance Requirements Analysis phase is a great opportunity to visit the assumptions being made, as the right questions and validate the underlying infrastructure capacity to be able to meet your Non Functional Requirements.
* **Get Buy in From you Customer and Team Leads** – For the success of the program and the Performance Engineering work stream it is important that you focus not just on the Non Functional Requirements but also the humane side of Performance. This is where a lot of program falter. Doing a great job on gathering the Non Functional Requirements is absolutely great but doing that in isolation without the buy in of your development leads, work stream lead and customer isn’t going to get you very far. As a Practical Performance Analyst you will find yourself setting up and conducting numerous workshops to bring together all your relevant stake holders with the objective of explaining to them the Non Functional Requirements and the expectations you have from each of them with regards to meeting those documented requirements.
* **Determine Tools, Resourcing, Infrastructure, Licensing requirements** – The Performance Requirements Analysis phase is a wonderful opportunity for you to establish yourself as the Performance Engineering SME on the program and help identify the tool, resourcing, infrastructure and licensing requirements on the program based on the documented Non Functional Requirements. A lot of work would have gone into defining the Non Functional Requirements before you would have been able to call out all the tooling, resourcing and infrastructure requirements. As a Practical Performance Analyst this is your best opportunity to document your requirements, call them out and work with the program leadership on obtaining access to the relevant tools required to get the job done.

### What are the activities involved in Performance Requirements Analysis

Performance Requirements Analysis is the first and most important activity in the Performance Engineering Life Cycle. As a Practical Performance Analyst you will pay a lot of attention to tasks at this stage ensuring that you’ve done a thorough job on defining the program Non Functional Requirements. The Non Functional Requirements you draft will have a major impact on the total program costs and overall End User Experience the business intends to deliver. The importance of this phase can’t and shouldn’t be underestimated.

![Performance Requirements Analysis]({{ "/assets/img/pe_requirements_analysis.png" | absolute_url }})

* **Review Business Requirements Document** – Performance Engineering might sound very technical in nature but it’s all about meeting enabling IT to meet business goals. As the Practical Performance Analyst it’s very important that you understand the business case and the business requirements to a fair extent and have spent time understanding the program objectives including the reasons for investment in the new solution or platform. You would like to start off with a strong understanding of the mistakes made in the past and business’s plans for the future. It’s the Practical Performance Analyst’s responsibility to understand translate the business requirements and help business articualte Non Functional Requirements that would be used to define the programs objectives and goals from a Non Functional standpoint.
* **Data Gathering** – At this stage you are just learning about the program, it’s overall objectives and goals. Get your hands dirty with all the relevant program documentation you can find to understand what the program objectives, the business case, is being designed, what approaches are being used and what are the platforms being used to deliver the solution. Gather as much as you can on the architecture, solution, development platform, deployment platform, etc.
* **Review Production Performance Metrics** – This is applicable only to programs where there is an existing version of the application in production. Having an application in production (older release) makes it a lot more easier for the Practical Performance Analyst as you are able to go in and extract all the relevant business & system performance metrics. Note my saying business and system performance metrics. It’s very important that you understand the business workload and infrastructure workload on the production systems. You should then ask for the relevant business workload and application workload data to be extracted from the production environment. Defining your Non Functional Requirements becomes a lot more easier once you have good visibility of the relevant business and infrastructure workload metrics.
* **Understand Business Objectives & Goals** – The Practical Performance Analyst needs the buy in from Business (customer) sponsor to be successful in the role of the lead Performance Engineer. In your discussions with business you would like to extract information about past performance issues, business growth over the last few years, expected business growth, business initiatives that have impacted platform performance in the past, business’s expecations from the new platform, end user experience issues they might already know of and any generic performance and capacity constraints they have been witness to.
* **Understand the view of the Program Architects & Solution Leads** - Speak to the program architects and solution leads to understand the solution approach and design patterns being used on the program. With knowledge of the solution, development platform and deployment platform you will be better positioned to fine tune your Performance Engineering approach for the program.
* **Obtain the Infrastructure View** – Obtain a view of the sizing guidelines your infrastructure support team (if one exists) or the application vendor (COTS application) have provided. Look around for sizing estimators, reach out to the Capacity Management experts in the field and get them to review the sizing guidelines or better still go and build some capacity planning expertise that will stand you in good stead for the longer term. If sizing estimates do not exist we would highly recommend reaching out to the vendor (in case of COTS) or to your capacity management guru to help you identify the capacity required to meet business workload.
* **Obtain a view of the existing tool landscape** – To deliver the program the Practical Performance Analyst needs access to several tools i.e. data visualization tools, performance modelling tools, performance testing tools, performance monitoring tools and capacity managemetn tools. You would need to assess the tool landscape, understand the breadth of tools available within the organization and then plan to put in a request for additional tools or licenses to bridge those gaps.
* **Practice being Practical** – It’s easier said than done and this is something that each one of us as a Practical Performance Analyst battles on a daily basis. You’ll be faced with numerous challenges and will need to compromise on various aspects. When you have to do so perform a detailed risk analysis, review the approach and revise it if necessary and present the findings. Make sure all your stake holders understand the implications of the decisions being made and how it would impact the Performance Engineering teams’ ability to validate the documented Non Functional Requirements.

### What are some of the challenges Involved in Performance Requirements Gathering

Here’s a summary of the challenges you are bound to face when involved in Performance Requirements Analysis.

* Challenges finding the right business and IT stakeholders
* Lack of understanding of Performance Engineering and the value it delivers across the Software Development Life Cycle
* Lack of production metrics for business and infrastructure workload
* Lack of access to the production systems to extract relevant business & infrastructure workload metrics
* Lack of Industry standard tools to analyze, model and visualize data for purposes of defining Non Functional Requirements
* Lack of Capable Resources to assist with data extraction, visualization and analysis


### Going about the Performance Requirements Analysis process 

So now you have a good understanding of the overall Performance Requirements Analysis process it's time to get started with the actual work.

You would ideally start with reviewing the "Business Requirements Document" if one exists and has been written. If not we would highly recommend reaching out to the various senior stakeholders on the program to understand the expectations from a Non Functional Requirements standpoint. If it's just initial days you might want to keep in mind that without signed off Business Requirements you do not really have much to base your Non Functional Requirements scope on. But if you have to absolutely kick off your Architecture/Performance related activities we would recommend reaching out to your peers across the business to understand the nature of Non Functional Requirements the system might consume based on similar systems that might have been delivered in the past. You will however want to go back and refine your thinking once you have a better view of the final set of Non Functional Requirements.

Secondly, when considering Non Functional Requirements have a think of all the relevant types of Non Functional Requirements depending on the nature of your clients business and the business process activities the system is being built to support. For critical systems you might have a larger set of core Non Functional Requirements covering End User Experience, System Utilization, Availability, Reliability, Security, High Availability, etc., while for lesser in-house non-customer facing non-critical systems you might only possibly have to factor in Non Functional Requirements around End User Experience, System Utilizations and System Availability. Do your homework and understand your clients business, including the business processes the system being built will support. With a good understanding of the processes and business you will be better placed to put together a view on the required Non Functional Requirements.

Where possible review the existing system in production to understand it's compliance with the set of laid down Non Functional Requirements. Many a times, clients enforce higher SLA's for system upgrades when the core of the system i.e. architecture, design, etc. isn't changing making it very difficult if not impossible for you to meet those requirements. When desiging a new system you will have a lot of flexibility to work through the Non Functional Requirements and negotiate with business on the ones that are most relevant.

In the end keep in mind that the more stricter and broader (in terms of coverage) your Non Functional Requirements are, the higher the cost of building and engineering the solution to meet those Non Functional Requirements. An architects or Performance Engineers role is to make sure you have the right balance of requirements required to meet the program goals. 

### Deliverables - Performance Requirements Analysis 

Deliverables for the Performance Requirements Analysis stage are provided below. We intend to include reference templates for each of the deliverables listed below at some point in the future.

* Performance Engineering Strategy
* Non Functional Requirements Document
* Confirmed list of Business & Infrastructure Workload Drivers
* Workload Gathering Questionnaire
* High level Performance Testing approach

### Resources 

Here’s a list of important resources on Performance Engineering :

* [Dr. Rajesh Mansharamani on Performance Requirement’s Analysis]( https://sites.google.com/site/swperfengg/home)
* [CMG Paper on Performance Requirements Analysis](http://www.cmg.org/measureit/issues/mit23/m_23_2.html)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

