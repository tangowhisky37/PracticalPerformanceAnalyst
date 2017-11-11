---
layout: pagelayout
title: Capacity Mangement 101
---

This section will delve into the various aspects of Capacity Management (also called Capacity Planning) as seen from the eyes of the Practical Performance Analyst (some one like yourself). The sections we intend to cover are -

* What is Capacity Management
* Why is Capacity Management Important
* What are the ITIL Sub Processes involved in Capacity Management
* What are the Activities involved in Capacity Management
* What are the Modelling techniques involved in Capacity Management
* Challenges involved in Capacity Management
* Deliverables for Capacity Management
* Tools for Capacity Management
* Resources on Capacity Management

### What is Capacity Management

Capacity Management is the discipline that ensures IT infrastructure is provided at the right time in the right volume at the right price, and ensuring that IT is used in the most efficient manner. This involves input from many areas of the business to identify what services are (or will be) required, what IT infrastructure is required to support these services, what level of Contingency will be needed, and what the cost of this infrastructure will be - [Link](http://www.itlibrary.org/index.php?page=Capacity_Management)

![Capacity Management Cycle]({{ "/assets/img/capacity_management_cycle.png" | absolute_url }})

Capacity Management is part of the overall ITIL process and is aimed at ensuring that applications have the required infrastructure capacity to meet the business and IT SLA’s while making optimal use of the underlying hardware platform.

In the following sections we’ll look into the details of Capacity Management and why on-going Capacity Management is important for the success of any small and large business.

### Why is Capacity Management Important

Capacity Management is important for the following reasons-

* Ensure that business is able to service its customer needs by delivering the expected End User Performance across all its business critical customer facing applications
* Ensure that the applications are able to meet its IT & Business SLA’s from a Performance & Availability standpoint
* Ensure Optimal Utilization of underlying hardware infrastructure
* Ensure enough of hardware infrastructure is available for the application to meet the documented End User Performance Requirements
* Give the business enough of lead time to procure additional infrastructure to meet increasing business workloads as required
* Ensure that IT has an agreed process to analyze current business & infrastructure workloads and forecast change in application performance for increase in business workloads (based on forecasted business growth and various business initiatives)
* Ensure that IT has an agreed process to determine additional infrastructure requirement to meet increasing business workloads

![Capacity Management Process]({{ "/assets/img/capacity_management_process.png" | absolute_url }})

### What are the ITIL sub processes involved in Capacity Management

This can be looked at from a few different perspectives. From a process standpoint there are numerous sub processes and tasks involved in Capacity Management and the process flow diagram will summarize the overall Capacity Management process. However, when looked at from an ITIL perspective Capacity Management can be further sub-divided into three sub processes.

* Business Capacity Management
* Service Capacity Management
* Resource Capacity Management

Let’s briefly go over the objectives of each of the sub-processes from a Capacity Management standpoint.

![Capacity Management Process - Input/Output]({{ "/assets/img/capacity_management_process1.png" | absolute_url }})

* **Resource Capacity Management** – The objective of this part of the ITIL sub process is to ensure that IT infrastructure is optimally utilized. This includes definition of optimal utilization levels or SLA’s for your entire production application infrastructure, ensuring you’ve got the appropriate monitoring tools in place to capture network/OS/application/transactional performance metrics and then being able to use them to analyse and manage your SLA’s from a Resource Capacity perspective. Resource Capacity Management sounds easy but the challenges customers face today are due to the various silos of data created by different monitoring tools that do not talk to each other.
* **Service Capacity Management** - The objective of this part of the ITIL process is to ensure that capacity levels across all production infrastructure, allow IT to meet the defined and agreed SLA’s. Large number of organization around the world, have adopted ITIL (or relevant parts of it) to streamline operations across IT. Service Capacity Management is a proactive measure geared towards ensuring capacity levels are in line with growing business workloads.
* **Business Capacity Management** – The objective of this ITIL sub process is to be able to forecast and provide business the required infrastructure capacity to be able to sustain growing business workloads. Business workloads can vary based on seasonal patterns, marketing initiatives, economic and social factors, etc. Business Capacity Management is aimed at ensuring IT works closely with business to ensure all business critical applications have the required capacity to meet current and future business workloads.

Capacity Management is an on-going process and never stops. As a Practical Performance Analyst it’s important to keep in mind the overall objectives of the Capacity Management process, understand the customer maturity levels, identify the business challenges and then craft a customized Capacity Management process that works for your customer. Take what we’ve documented here as a set of guidelines and customize them to suit your individual requirements.

### What are the Activities involved in Capacity Management

The activities involved in Capacity Management are listed below-

* Understand application architecture
* Understand existing application performance & scalability issues
* Document Business Workload (Txns/Hour, Messages/Hour, etc)
* Document Infrastructure Workload (CPU Utilization, Memory Utilization, etc)
* Identify sources for Business & Infrastructure Workload
* Extract Business & Infrastructure Workload
* ETL Business & Infrastructure Workload into your Capacity Management solution
* Create your performance & capacity models
* Obtain details around business growth for your keep Business Workload Drivers
* Model application performance for key  Business Workloads and identify Capacity impacts
* Publish Capacity Management reports
* Publish Infrastructure Capacity recommendations
* Work with your application teams on detailed capacity plans for the affected tiers
* Monitor application performance and repeat steps mentioned above

This list is by no means a comprehensive list of activities but should provide you with a set of guidelines you can use to setup your Capacity Management process. As a Practical Performance Analyst you should be focussed on understanding the business goals while keeping in mind how much you customer values performance and how much he/she is willing to spend on addressing Performance issues across their production applications.

### What are the Modelling techniques involved in Capacity Management

Capacity Management has been rocket science for most organizations and at the Practical Performance Analyst we’ll do our best to debunk that myth. Over the next few months and years we’ll put together a set of articles and techniques that will help you setup Capacity Management across your organization without having to blow a hole in your pockets. You don’t really need million dollar tools to address Capacity Management but what you’ll need is an excellent understanding of the different data visualization, data analysis, statistical modelling tools to be able to perform Capacity Management.

This section will summarize the different modelling techniques required to perform on-going Capacity Management-

* **Data Analysis & Visualization techniques** –
  * Time Series Analysis
  * Scatter plots
  * Q-Q plots
  * Box Plots
  * Histograms
  * Frequency & Bar chards
* **Performance Modelling techniques**
  * Statistical modelling
    * Time Series Forecasting
      * Holt Winters Forecasting methods
      * ARIMA Forecasting methods
      * Time Series Decomposition
      * Time Series Moving Average
      * Exponential Smoothing methods
  * Analytical modelling
    * Queuing Theory
    * Queuing Networks
    * Petri Nets
    * Markov’s Chains
  * Simulation modelling
    * Discrete Event Simulation models

We will delve into the details of identifying the appropriate methods and using the relevant methods for Performance Modelling & Capacity Management. As a Practical Performance Analyst we would recommend that you visit the recommend list of reading books as documented at the Practical Performance Analyst and start picking up on the basics of Data Mining, Data Visualization, StatisticsMathematics required to perform Capacity Management. There are quite a few million dollar solutions available out there but as a Practical Performance Analyst, we’ll help you perform Capacity Management without any of the expensive solutions using simple and easy to obtain tools.

### Challenges involved in Capacity Management

Here’s a summary of the challenges we’ve had to face from a Capacity Management perspective-

* Lack of monitoring tools to capture relevant application, network, infrastructure performance metrics
* Lack of data store including historical data for performance monitoring metrics
* Lack of sophisticated tools for Capacity Management
* Lack of understanding of Performance Engineering & Capacity Management concepts across the organization
* Lack of skills required for Performance Modelling & Capacity Management
* Lack of understanding of business workloads for your key business critical applications
* Challenge obtaining forecasts for business workloads from relevant areas of business
* Challenge identifying & extracting business workload data from production environments (most application’s aren’t built to log relevant business workload metrics)
* Challenge getting a buy in from various stakeholders on the need to invest in Capacity Management process
* Inaccurate business and infrastructure workload data due to work around implemented to capture relevant workload metrics

### Deliverables involved in Capacity Management

The deliverables for the Capacity Management process are listed below-

* Performance models for your key business critical applications and application tiers
* Capacity Management Reports – Generally monthly or in large organizations Quarterly
* Capacity Plans for impacted applications – Details about infrastructure required

### Tools for Capacity Management

* BMC Capacity Management - [Link](http://www.bmc.com/products/product-listing/capacity-optimization.html)
* TeamQuest Capacity Management - [Link](http://www.teamquest.com/products-services/teamquest-performance-software/index.htm)
* CA Capacity Manager - [Link](http://www.ca.com/us/capacity-manager.aspx)
* Quest Foglight Virtualization Capacity Manager - [Link](https://www.quest.com/products/foglight-for-virtualization-enterprise-edition/)

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

