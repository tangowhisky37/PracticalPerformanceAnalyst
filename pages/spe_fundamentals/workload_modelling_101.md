---
layout: pagelayout
title: Workload Modelling 101
---

This section will define the concept of Workload Modelling and delve into details around Workload Modelling as seen from the eyes of the Practical Performance Analyst (some one like yourself). The topics we intend to cover in this section are –

* What is Workload Modelling
* Need for Workload Modelling
* Variation in Workload Modelling techniques
* Why Workload Modelling is so important
* Activities involved in Workload Modelling
* Challenges involved in Workload Modelling
* How-To’s on Workload Modelling
* Deliverables on Workload Modelling
* Resources on  Workload Modelling

### What is Workload Modelling 

Let’s start out by defining Workload and then move onto the subtle differences in Workload modelling for different aspects of Performance Engineering across the Software Development Life Cycle. Workload can simply be defined as a logical set of activities that need to be performed by users (business or customers using the system) towards achieving a certain (business or customer) goal. As a Practical Performance Analyst I would tend to characterize Workload into two main areas, Business Workload and Infrastructure Workload.

* **Business Workload** – Business Workload is the logical set of activities that need to be performed in order to meet the business objectives and goals. As a Practical Performance Analyst you are expected to have a solid understanding of the customer’s business, his business model, what makes the business tick, what are the different business initiatives that will impact performance of the platform including the different relevant aspects of Business Workload you need to consider on your program. Business Workload would imply different things for different businesses and different individuals within the same business. For example let’s take an online retail business. For the online retail business the business workload on its applications would include – Page Views/Hour, Orders Submitted/Hour, Mails Sent To Customers/Hour, etc. For a business with interests in the online retail banking space the workload would include – Page Views/Hour, Check Account Balance Transactions/ Hour,  Withdraw Money Transactions/Hour, Messages to the Core Banking System/Hour, etc.  Business Workload differs from one customer to the other and even across business units within the same customer based on the nature of the task being performed and the application that has been designed to address the task. Simply speaking Business Workload consists of a logical set of activities that need to be performed by the application in order for the business or customer to meet its stated objectives and goals.
* **Infrastructure Workload** – Infrastructure Workload on the other hand is relatively easy to understand and appreciate. As a Practical Performance Engineer Infrastructure Workload consists of the logical units of work, that are performed by the underlying Infrastructure to process Business Workload. Infrastructure Workload very simply put includes the following – CPU Utilization/5mins, Memory Utilization/5mins, IO Operations/5mins, etc. Infrastructure Workload should complement Business Workload and in most cases would have a strong relationship with Business Workload drivers for a given application. Later in this foundation series we will be looking at modelling Business Workload & Infrastructure Workload to be able t forecast performance of the applications and identify infrastructure capacity impacts.

### Need for different Workload Modelling techniques

Workload modelling techniques would differ slightly based on the activity you are engaged in across the Performance Engineering life cycle. As a Practical Performance Analyst I have found myself having a few different views on the Workload modelling techniques required depending on the nature of the program and the objectives of the Performance Engineering assignment I have been working on. Some of the Practical Performance Analysts out there might argue that all you need is probably just one version of the Workload model irrespective of the Performance Engineering activity (Performance Testing, Performance Modelling, Capacity Management, etc) you are involved with but then again every man unto himself (or woman unto herself…J).

Experience has told me that this isn’t the case and most of the times it just not practical to over simplify Workload models and collapse all detail into one single large common Workload model which not only doesn’t serve the purpose but also goes a long way to confuse the end consumer of the model i.e. the customer performance testing or capacity management teams.In instances where the workload is really simple you could indeed get away with just one version of the Workload model for different Performance Engineering activities but in instances where the applications are really large and complex you will need to invest in building separate custom workload models for the different Performance Engineering activities across the Software Development Life Cycle.

One of the reasons I also recommend you have different Workload models is to simplify the interpretation of those Workload models given the different teams you are engaged with across the customer site. Performance Testing teams don’t generally have any understanding of Capacity Management and less and understanding of Performance Modelling techniques. You’ll do yourself a big favor by being Practical and focusing on building custom Workload models based on the tasks at hand and the customer teams you will be involved with.

### Variation in Workload modelling techniques

Workload modelling techniques as mentioned earlier could vary depending on the Performance Engineering activity and the objectives of the program you are involved with. The most complex Workload models in our experience are required for purposes of Performance Testing or SVT (Stress Volume Testing) while Capacity Management Workload models tend to be easier to design. **Please don’t confuse Workload models with Capacity Models or actual Application Performance models which are two completely different things.**

Let’s have a brief look at the different Workload models and what is their relevance from a Practical Performance Analyst’s standpoint. Workload models for Performance Testing ideally require you to gather the following Workload data from the perspective of documenting the various aspects of the Business Workload along with the accompanying Non Functional Requirements to be used as Performance Testing objectives on the engagement –

* User Concurrency Targets
* Transactional Workload (OLTP Workload)
  * Throughput Targets
  * Response Time Targets
  * Think Time Assumptions
* Messaging Workload
  * Throughput Targets
  * Response Time Targets
* Workflow Workload
  * Throughput Targets
  * Response Time Targets
  * Think Time Assumptions
* Batch Workload
  * Duration Targets
  * Volume processed Targets

Workload modelling for purposes of Performance requires use of Little’s Law which will be dealt with in a lot more detail in Little’s Law to be covered later in this foundation series. The objective of designing the Performance Testing workload models is to ensure that all the Performance Testing Engineers, support teams, development teams and design teams clearly understand the Workload for the System Under Test (SUT) and have the ability to transform the Performance Testing Workload models directly into designs for Performance Testing Scenarios in their Performance Testing tool (e.g. HP Load Runner, Radview Webload, etc).

![Workload Modelling Process]({{ "/assets/img/workload_modelling_process.png" | absolute_url }})

However, workload models for Performance Modelling and Capacity Management are quite different. These workload models typically list down all the various Business and Infrastructure workload drivers required for purposes of Performance Modelling and Capacity Management along with details about availability, type, format and location of the required data for all of the identified workload metrics. In the workload models for Performance Modelling and Capacity Management you would ideally only provide a list of key Workload drivers and would essentially capture the following data –

* User Concurrency – Actual Production Values
* Transactional Workload (OLTP Workload)
  * Throughput – Actual Production Values
  * Response Time – Actual Production Values
* Messaging Workload
  * Throughput – Actual Production Values
  * Response Time – Actual Production Values
* Workflow Workload
  * Throughput – Actual Production Values
  * Response Time – Actual Production Values
* Batch Workload
  * Duration – Actual Production Values
  * Volume processed – Actual Production Values

We will delve into the details of Capacity Management & Performance modelling later in this foundation series. None of the above lists are meant to be exhaustive in nature but are meant to give you an understanding of the subtle difference in Workload modelling and data collection techniques for different Performance Engineering activities across the Performance Engineering Life Cycle. Having separate workload models helps you state your case a lot more clearly and helps you speak to the different client teams in their own languages.

### Why Workload Modelling Is Important

Workload modelling is essentially part of the data collection and requirements gathering process within the Performance Engineering life cycle. Workload modelling is essential for a good amount of reasons. They are listed as follows –

* **Performance Testing**
  * Helps you confirm the Performance Engineering teams assessment and understanding of critical Business & Infrastructure Workload drivers that impact platform performance and hence infrastructure capacity
  * To give you a good understanding of the OLTP Transactions, Batch jobs, Messaging & Workflow workload to be considered in your scenario designs
  * Makes it easy to communicate to business and your other internal stake holders how you intend to model your different scenarios
  * Helps you translate your Non Functional Requirements into Performance Testing SLA’s
  * Gives you a great opportunity to get a buy in from your business users and other internal program stake holders on what should be and needs to be considered for purposes of Performance Test
  * Is another tick in the box in your requirements matrix confirming you’ve covered the relevant aspects of business requirements for Performance Test
* **Performance Modelling & Capacity Management**
  * To give you a good understanding of critical Business & Infrastructure Workload drivers that impact platform performance and hence infrastructure capacity
  * To give you a good understanding of the OLTP Transactions, Batch jobs, Workflows and Messaging workload to be considered for purposes of modelling
  * Makes it easy to communicate to business and your other internal stake holders what you are considering as key inputs to the various modelling techniques
  * Gives you a great opportunity to get a buy in from your business users and other internal program stake holders on what should be and needs to be considered for purposes of modelling

### What Are The Activities involved in Workload Modelling

The activities involved in Workload modelling are as follows:

* Understand Business Objectives & goals from a program point of view
* Grab hold of the business case if possible and familiarize yourself with business’ aspirations for the new platform or solution
* Understand solution approach from a technology standpoint
* Speak to business and customers to understand pains the customers are facing with the existing application
* Speak to business and customers to understand reasons and drivers behind the current initiative
* Work with business to nail down critical Business Workload
* Work with IT to nail down critical Infrastructure Workload
* Work with the application SME’s to map the business workload to different pieces of functionality across the application and identify data stores for the workload metrics
* Work with the systems administrator to map the infrastructure metrics to the different monitoring metrics as being captured by monitoring tools
* Map Non Functional requirements to aspects of your workload as required
* Extract, clean, transform data for purposes of workload analysis
* Put together your workload models and review with business and IT
* Workshop your workload models with all your stake holders including business and internal work stream leads
* Obtain sign off from all of your stake holders confirming their understanding of the truth as it exists

### Challenges Involved in Workload Modelling

Modelling Workload has its own set of challenges. Listed below are the challenges we have encountered over the years trying to put together sensible workload models for programs worldwide. This list isn’t meant to be exhaustive is nature but is rather intended to give you an glimpse of the challenges you are likely to face when embarking on Workload Modelling for Performance Test, Application Performance Modelling or Capacity Management.

* Getting access to relevant business users who have a strong understanding of the business workload
* Getting access to application SME’s who have a strong understanding of the application and its functionality
* Getting access to the existing applications to extract data for purposes of workload analysis
* Unable to get access to data for workload analysis since the existing application do not log relevant business workload metrics
* ETL (Extract, Transform & Load) of the data from different exotic data sources into a format that could be used for Workload analysis
* Access to tools that could help you automate ETL of business and infrastructure workload data due to the large volumes of information that need to be parsed
* Finding the right business and application SME skills required to translate workload metrics (extracted from the system) into sensible data for purposes of workload analysis
* Convincing your different stake holders that Workload modelling isn’t rocket science and is a necessary investment for the Performance Engineering team to have a strong understanding of production workload to be able to design sensible Performance Testing scenarios that validate the documented Non Functional Requirements (NFR’s)

### How-To’s on Workload Modelling

Watch this space for detailed HowTo’s on Workload modelling for Performance Testing, Performance Modelling & Capacity Management.

* Modelling Workload for Performance Testing  (Application of Little’s Law)
* Modelling Workload for Capacity Management & Performance Modelling

### Deliverables from Workload Modelling process

Deliverables from the Workload Modelling process include the following. Templates for the same will be provided in the near future. –

* Performance Testing Workload Models
* Capacity Management Workload Models
* Workload models for Application Performance Modelling

### Resources on Workload Modelling

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

