---
layout: pagelayout
title: What Is Service Time
---

Let's start by taking a look at the definition of Service Time. 

### Service Time or St

Service Time or St is simply defined as the time taken by the system to process a particulate service request. Service Time tends to remains constant for a given transaction when there is no change in any of the user inputs or other environment variables that govern the performance of the given business transaction.

Lets revisit our basic equation for Response Time:

  * Rt = Wt + St &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;.  [ Wt = Wait Time, St = Service Time ]  **_also written as_**
  * Rt = Qt + St  &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;.  [ Wt = Wait Time, Qt = Queuing Time ]

Service Time is the constant in the above equation for a given set of input parameters. What generally causes the Response Time to vary is the Queuing Time [Qt] or Wait time [Wt] variable which depends on various factors including congestion at a given resource, sudden increase in demand for a given resource, etc. Service Time like overall response time can be measured at the Network tier, Hardware tier, Disk tier, CPU tier, etc. is a known constant.

Thus next time around when someone suggests degradation in Service Time for a given business transaction what they are actually implying is that the Response Time for the given business transaction has degraded due to increase in the Waiting Time for computational resources required to process the given transaction. Service Time in this case will remain a constant as long as there is no change in any of the input variables or volume of data provided as input.

### Service Time Equation 

Service Time for a given resource can also be modeled using some very basic Performance equations. Lets look at the following scenario.

  * We start watching a system at t=0 and end viewing of the system at time t=T
  * The duration for which the system has been busy is described by Bt
  * During the time T there were C Completions (successfully processed transactions)
  * The Service Time for a particular transaction can thus be defined as:
  * St = Bt / C ...... [ Bt = Busy Time, C = Completions ]

**Example** _Lets say we have observed a system for 60 seconds and within the 60 seconds the system has had 15 Completions or 15 successfully exited customers._

_We know &#8211;_ St = Bt / C ........ [ Bt = Busy Time, C = Completions ]

_The Service Time each customer can be calculated as: _ _Service Time or St = 60  / 15 = 4s_

We have chosen to apply the above scenario to an overall system but this could also be applied to a component within an existing system. The Service Time equation is one of the most basic equations used to identify the service time for a given resource within a system or even the system as whole.


### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

