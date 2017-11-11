---
layout: pagelayout
title: Performance Modelling 101
---

This section will define the concept of Application Performance Modelling and delve into details around Performance Modelling as seen from the eyes of the Practical Performance Analyst (some one like yourself). The topics we intend to cover in this section are -

* What is Performance Modelling
* When would i use Performance Modelling
* What aspects of Performance should i be Modelling
* Why is Performance Modelling important
* Activities involved in Performance Modelling
* Challenges involved in Performance Modelling
* Deliverables from the Performance Modelling process
* Tools for Performance Modelling
* Resources on Performance Modelling

### What is Performance Modelling

Performance Modelling is the process of modelling application performance considering various growth factors with the objective of proactively predicting potential breach of SLA’s. Performance iModelling is also used to validate design decisions and infrastructure investment decisions at development stage.

This definition though is a very vague definition and is provided for purposes of simplicity. When looked at from the eyes of a Practical Performance Analyst, Performance Modelling is a science that very clearly fits into the proactive performance paradigm and can be applied across the Software Development Life Cycle. The various areas phases where you could chose to apply Performance Modelling is listed below –

* Performance Modelling at Requirements Gathering
* Performance Modelling at Design
* Performance Modelling at Performance Test
* Performance Modelling at Go Live
* Performance Modelling when in Production

As a Practical Performance Analyst you should be looking to use Performance Modelling techniques to validate decisions and predict potential impact on applications and infrastructure performance in a proactive manner.

When would I use Performance Modelling - Performance Modelling offers a set of modelling techniques that should be used across the Software Delivery Cycle. Unfortunately so far, most of this has been rocket science and the few tools out there that claim to provide the modelling capability are themselves quite challenging to learn and implement. Over the next few years, here at the Practical Performance Analyst we will attempt to change that. We will bring you the best of the tools in the Performance Modelling space, simplify the process of Performance Modelling and help you as a Practical Performance Analyst understand what your options are and how should you go about modelling performance of your application and validating the decisions being made early in the Software Development Life Cycle.

Listed below are key phases across the Software Development Life Cycle where you could choose to use Performance Modelling techniques to validate your decisions and predict potential change in application performance.

### Performance Modelling at Requirements Gathering

At requirements gathering stage performing the role of the Practical Performance Analyst your focus is to determine the overall Non Functional Requirements across the application. As part of this role you’ll focus on identifying key business and infrastructure workload across the various tiers and obtain an understanding of the user workload that drives utilization and hence application performance across the various application tiers. At this stage you have the opportunity to use Analytical and Simulation Modelling techniques to validate your Non Functional requirements. At this stage you don’t have infrastructure specifications for your applications yet but you should be in a position where you can start looking at feasible options and recommend sizing guidelines based on your understanding of the Non Functional Requirements, business workload, infrastructure workload, operational SLA’s and your experience managing performance across clients.

![Application & Infrastructure View Of Performance]({{ "/assets/img/performance_triangle.png" | absolute_url }})

* **Performance Modelling at Design** – At design stage, you have high level and detailed design specifications now made available to you. This is a wonderful opportunity to get hold of the design specifications, application architecture, and deployment architecture to validate the various decisions. You can use a combination of Analytical and Simulation Modelling techniques at this stage to validate the ability of the application architecture and underlying infrastructure to meet the overall Non Functional Requirements.
* **Performance Modelling at Performance Test** – At Performance Test you would have started generating good amounts of statistical data through the various Performance Testing runs. As a Practical Performance Analyst you should use this as an opportunity to use a combination of different Statistical, Analytical and Simulation Modelling techniques to validate the scalability of the application. Your ability to use Statistical Modelling techniques at this stage is a key advantage in predicting application performance for growth of key workload drivers while being able to call out potential breaches in operational SLA’s. Statistical Modelling techniques tend to be easier to use, require you to make fewer assumptions and are easy to build and implement. Statistical Modelling techniques are also very useful when you have gaps between the size of your performance testing and production environment and need to extrapolate the performance and scalability of your systems based on performance testing results.
* **Performance Modelling at Go Live** – At go live you could use Statistical Modelling techniques to understand performance of the application and predict potential breach in operational SLA’s for a given combination of infrastructure and software configuration. Statistical Modelling techniques are easy to apply and using data generated from Performance Testing you should be in a position where you can forecast application performance and infrastructure utilization for growth in business workload. You can also use a host of Analytical and Simulation Modelling techniques to understand changes in application performance for growth of different business workload drivers.
* **Performance Modelling when in Production** – When in production you have started generating large amounts of data (assuming you have instrumented your applications well and have started collecting infrastructure workload and business workload data) and should be able to use Statistical Modelling techniques to identify relationships between your business workload drivers and infrastructure workload drivers for the business critical applications with the objective of forecasting potential impacts to application performance. You could also use a combination of Analytical and Simulation Modelling techniques to validate what-if scenarios for changes in infrastructure specifications or application configuration. Statistical Modelling techniques can be used to predict change in application performance when your baseline hasn’t changed i.e. when your software configuration, OS configuration, hardware configuration, etc. is constant and hasn’t changed. For what-if analysis in scenarios where you need to understand application performance for different hardware and software configurations you would need to use a combination of Analytical and Simulation Modelling techniques.

### What aspects of Performance should I be Modelling

As a Practical Performance Analyst you should be keen to understand variation in application performance for growth of key workload drivers.  You should be keen to understand the following performance metrics for change in business workload, infrastructure specifications and software configuration -

* Transactional Response times
* Utilization levels across the different tiers
* Queue length across the various different tiers
* Wait time across the different tiers
* Services times across the different tiers

Performance modelling should be ideally performed on a continuous basis across the Software Development Life Cycle with the objective of identifying changes in application behavior due to key design, infrastructure or configuration changes.

### Why is Performance Modelling Important

Performance Modelling offers a set of techniques that give you the Practical Performance Analyst the opportunity to understand change in application performance for variation in business workload including the ability to predict application performance based on key design and infrastructure decisions. We’ve put together what we think are reasons why Performance Modelling is important across the Software Development Life Cycle –

* Understand end user performance at design
* Validate design decisions
* Provide guidelines for infrastructure sizing
* Validate infrastructure specifications
* Extrapolate application performance using data from performance test
* Forecast application performance using data from production environments
* Predict change in application performance for growth in business workload
* Determine infrastructure impacts due to growth of business workload
* Predict change in application performance due to change in software configuration
* Predict change in application performance due to change in infrastructure specifications

### Activities involved in Performance Modelling 

Performance Modelling is very similar to the workload modelling process we’ve covered earlier. Here’s the list of steps involved in modelling the performance of your applications –

* Determine Non Functional Requirements
* Understand Business Objectives & Goals
* Understand Application Architecture
* Understand Deployment Architecture (Infrastructure Platform, designs, etc.)
* Determine Business Workload
* Create Workload models (use workload modelling techniques)
* Obtain Performance data from existing applications in production (if possible)
* Extract data from production environments (if older versions of applications exist)
* Determine which modelling techniques are applicable
* Use a combination of modelling techniques and validate your results
* Present findings and use the findings to review your design decisions and infrastructure investment decisions

Performance Modelling is a science but applying it is an art. As a Practical Performance Analyst we would recommend you spend a few years working with an experience Practical Performance Analyst who could mentor you in using the different modelling techniques. We would also recommend investing in the Performance Engineering books recommended on the reading section of this website to gain a better understanding of the different modelling techniques and how you could apply them in the different scenarios across the Software Development Life Cycle.

### Challenges involved in Performance Modelling

A summary of the challenges in Performance Modelling is presented below –

* Lack of understanding of Non Functional Requirements
* Lack of details around Application Architecture due to poor documentation
* Lack of details around Infrastructure Specifications (you’ll be surprised how many support teams really don’t know what hardware they are using in production)
* Lack of buy in from various stake holders across the teams
* Lack of understanding of Performance Modelling techniques across the various stake holders
* Lack of software to automate Performance Modelling
* Lack of monitoring tools in production environment, hence inability to collect performance metrics
* Inability to extract business and infrastructure workload data from production environments
* Lack of tools to ETL business and infrastructure workload data for purpose of analysis
* Lack of analytics tools to analyze and visualize data extracted from performance testing and production environments

### Deliverables from Workload Modelling process

As part of on-going Performance Modelling you would like to present to your customers the following –

* **At Requirements Gathering** -
  * A report covering the following:
  * Realistic Non Functional Requirements
  * Infrastructure recommendations
  * Design recommendations
* **At Design** –
  * A report covering the following –
  * Performance models that highlight performance constraints
  * Validation of Application Architecture in meeting NFR’s
  * Validation of Infrastructure specifications
  * Validation of Design
* **At Performance Test** –
  * A report covering the following:
  * Forecasted performance for given business workload
  * Utilization levels for forecasted performance
  * Infrastructure impacts for given business workload
  * Impacts to customer experience for given business workload
  * Performance extrapolated for production environments
* **At Go Live** –
  * A report covering the following:
  * Forecasted performance for given business workload
  * Utilization levels for forecasted performance
  * Infrastructure impacts for given business workload
  * Impacts to customer experience for given business workload
* **In Production** –
  * A report covering the following:
  * Forecasted performance for given business workload
  * Utilization levels for forecasted performance
  * Infrastructure impacts for given business workload
  * Impacts to customer experience for given business workload

Look out for articles and howto's on Performance Modelling at the Practical Performance Analyst. We intend to cover various aspects of Performance Modelling from the viewpoint of a Practical Performance Analyst.

### Tools for Performance Modelling

Performance Modelling could be performed with several different objectives in mind, this could include, validation of the solution approach or solution architecture, validation of infrastructure requirements for a given solution approach and possibly impact analysis for change in business workload volumes. Application Performance Modeling can be performed using a combination of statistical, analytical and simulation modeling techniques. Unfortunately there aren't any standard commercial or Open Source tools out there for performance modeling. The list below suggest applications with their areas of focus.

* Anylogic (Discrete Event Simulation Modeling) - [Link](http://www.anylogic.com)
* IBM SPSS (Statistical Modeling) - [Link](http://www.ibm.com/software/au/analytics/spss/)
* JMT (Queuing Networks, Mean Value Analysis, Markov's Chains) - [Link](http://jmt.sourceforge.net/)
* Minitab (Statistical Modeling) - [Link](http://www.minitab.com/)
* R Project (Statistical Modeling & Data Visualization) - [Link](http://www.r-project.org/)
* Statsoft (Statistical Modeling & Data Visualization) - [Link](http://www.statsoft.com/)
* Simpy (Discrete Event Simulation Modeling) - [Link](http://simpy.sourceforge.net)
* Simul8 (Discrete Event Simulation Modeling) - [Link](http://www.simul8.com)
* TIBCO SpotFire S+ (Statistical Modeling) - [Link](http://spotfire.tibco.com/products/s-plus/statistical-analysis-software.asp)

### Resources on Performance Modelling

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

