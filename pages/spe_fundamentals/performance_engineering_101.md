---
layout: pagelayout
title: Performance Engineering 101
---

This section will define the concept of Software Performance Engineering and delve into details around Performance Engineering as seen from the eyes of the Practical Performance Analyst (some one like yourself). The topics we intend to cover in this section are –


* What is Performance Engineering
* Why is Performance Engineering Important
* What are some of the main activities involved in Performance Engineering
* What are some of the main challenges involved in Performance Engineering
* Designing your own Performance Engineering Strategy
* Key deliverables
* Resources

So lets dive into each of the topics listed above.

### What is Performance Engineering

Performance Engineering (SPE) is a systematic and quantitative approach for the cost-effective development of software systems to meet stringent Non Functional Requirements (Performance – Capacity – Scalability – Availability – Reliability – etc). Dr. Connie Smith in her book on Software Performance Engineering advocates that, Performance Engineering is a software-oriented approach, focused on optimal selection of application architecture, design, and implementation choices with the objective of meeting Non Functional Requirements. Software Performance Engineering can also be defined functionally as the set of tasks or activities that need to be performed across the Software Development Life Cycle (SDLC) to meet the documented Non Functional Requirements.Software Performance Engineering is often viewed as the art of building systems that meeting Non Functional requirements within the allocated time frame and budget constraints.

### Why is Performance Engineering Important

Performance Engineering is important for the following reasons.
* **Document & Validate Non Functional Requirements** – An investment in Performance Engineering strongly implies that you and customer intend to get things right the first time around. As part of Performance Engineering one sets out to define objectives and targets for the program under consideration. These requirements are mostly viewed as Non Functional Requirements that address various aspects of Performance, Reliability, Scalability, Availability, etc. Without targets there aren’t any objectives and without objectives you can’t have a plan. So Performance Engineering allows for some of the very basic elements and building blocks to be put in place early in the Software Development Life Cycle.
* **Low Impact & Cost of Change early in the cycle** – It’s comparatively easy to make changes to the application design and underlying infrastructure specifications at design stage to meet the documented Non Functional Requirements. Influencing the stake holders to agree to a change request that is aimed at ensuring the application meets its Non Functional Requirements is an easy sell at design stage.
* **Minimize re-work required to meeting NFR’s down the line** – Re-work at later stages of the Software Development Life Cycle (SDLC) can prove to be expensive, inefficient and time consuming, not saying it might even cost you your reputation. Re-writing parts of the application or requiring to re-consider certain design elements that would radically change the architecture of the application to meet the documented Non Functional Requirements is can prove to be a very expensive exercise once the team has progressed considerably with build.
* **Prevent things from going pear shaped in production** – Performance Engineering advocates proactive Performance & Capacity Management across the Software Development Life Cycle. Having Performance at the back of your mind in everything you do ensures that you have the right approach in identifying bottlenecks and concerns across the design, build and test phases thus drastically reducing the chances of you being caught unware with Performance or Scalability issues once you’ve gone live. Besides, your organizations reputation at stake think about the potential impact to customer experience.
* **Prevent the need for band aid fixes in production** – Not investing in Performance Engineering is the best way to begin applying band aid fixes in production. Of course, this is any program leads nightmare but is a very common situation across a lot of the customers i’ve work with so far. Building Performance Engineering initiatives into your program is the most appropriate way to avoid getting into a situation that forces you to consider applying band aid fixes in production.
* **Strengthen & enhance the relationship with your client** – What’s better that sipping a PinnaColada on the beach having a chat to your customer about the next big gig when you’ve just gone live with the current one. Of course, not all of us have the pleasure of finding ourselves in a situation such as what I’ve just described. Go live for most application development teams means long and pain ful weekend filled with working lunches and dinners that include pizza and coke. Unimpressive but this is what most of the software development projects have come down to. Based on our practical experience only a handful of my customers so far have been able to sit back and relax on d-day and that was mostly due to a rigorous Performance Engineering methodology advocating Proactive Performance Management across the Software Development Life Cycle.
* **Focus on the things that are important and prevent fire fighting** – Performance Engineering advocated Proactive Performance Management which ensures that programs leads and Performance leads on programs have the ability to focus on the important aspects of delivery. When Performance is part of the Software Development Life Cycle you’ve minimized your risk and have done your best to avoid things going pear shaped late in the program.
* **Metrics to measure and validate the end customer experience** – An investment in Performance Engineering ensures you’ve understood, documented and are able to track important customer metrics across the Software Delivery Life Cycle. This would mean different things to different programs from a Performance Engineering standpoint. But it’s important to be able to define, document and track relevant customer performace metrics from design to go live to be able to quantify the business benefits of the investment being made.
* **Spend wisely and get the most bang for your buck** – Proactive Performance Management ensures you’ve got the most for your investment by nipping potential issues early in the Software Development Life Cycle. The upfront start up costs on the program could prove to be higher but this needs to be viewed against the value the customer see himself or herself deriving by ensuring the program meets the goals stated in the business case. A good job on Performance also inevitably ensures that the customer goes smiling all the way to the bank.

### What are the main activities involved in Performance Engineering

Here’s a list of activities involved in the Performance Engineering Life Cycle. The Performance Engineering Life Cycle mirrors the Software Development Life Cycle and provides a set of key tasks to be performed at each phase of the Software Development Life Cycle.

![Performance Engineering Lifecyle]({{ "/assets/img/pe_lifecycle.png" | absolute_url }})

* **Requirements Gathering** – Document Non Functional Requirements and get client & team buy in. The Performance Requirements Analysis section will delve deeper into details.
* **Architecture & Design** – Design & Architect for high performance. Use various modelling techniques to validate the design assumptions from both an application design and infrastructure design standpoint.
* **Build** – Implement coding standards. Work with the development leads to implement guidelines focussed on validating and reporting unit performance for all the code being written.
* **Test** – Document your Performance Testing Strategy and validate the application for the documented Non Functional Requirements.Evolve your Performance Monitoring & Capacity Management strategy as you move through SVT.
* **Production** – Monitor your application and model the Application Performance with the objective of Identifying Infrastructure Capacity impacts. Call out the need to optimize the application / database to meet Non Functional Requirements or provision additional infrastructure to meet growing business workload.

### What are some of the key challenges associated with Systems Performance Engineering

Here’s a summary of the challenges you are bound to face when attempting to implement Performance Engineering across your program.

* Lack of funding to invest in Performance Engineering initiatives
* Lack of funding to invest in relevant tools to perform SPE activities across the life cycle of the project
* Lack of understanding of Performance Engineering and the value it delivers across the Software Development Life Cycle
* Lack of customer buy in for investment in SPE
* Lack of buy in from your own program and development leads
* Lack of Industry standard tools to model, visualize, validate, predict Performance & Capacity across the Software Development Life Cycle
* Lack of Capable Resources to build a strong Performance Engineering work stream on the program
* Insufficient time to invest in Performance Engineering initiatives due to strict program delivery schedule.

## Designing your own Performance Engineering Strategy  

Designing your Performance Engineering strategy for your program is important because it allows you to articulate to the leadership the investments in Systems Performance Engineering activities required across the delivery life cycle. Your assessment of the investment required would take into consideration the complexity of the system architecture, the nature of the business the customer is in, importance of meeting Non Functional Requirements (performance, scalability, reliability, high availability, etc.), how critical is the system to the survival of the business and the nature of investments the customer is willing to make to ensure the quality of service (as delivered by the system) doesn't deteriorate.

Here's some of the key dimensions you would consider when pulling together your Systems Performance Engineering strategy - 

- Scope of SPE for the program
- High Level Design & Non Functional Requirements
- Phases across the life cycle where SPE activities are applicable
- Integration of SPE activities with Design/Build/Test processes and tools
- Tooling required to support relevant SPE activities
- Resourcing required to support relevant SPE activities
- Overall outcomes SPE will deliver
- High level view of timelines for SPE activities on the program

### Key Systems Performance Engineering Deliverables

Deliverables from a Performance Engineering process are listed below. We intend to include reference templates for each of the deliverables listed below at some point in the future.

* Performance Engineering Strategy
* Workload Models
* Non Functional Requirements
* Performance Models
* Performance Testing Strategy
* Performance Monitoring Strategy
* Capacity Management Strategy
* Capacity Plan
* Technical Architecture / Design review & reccomendations

### Additional Resources

Here’s a list of important resources on Performance Engineering :

* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 
