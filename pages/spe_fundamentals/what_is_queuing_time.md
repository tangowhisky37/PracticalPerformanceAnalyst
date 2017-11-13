---
layout: pagelayout
title: What Is Queuing Time
---

### Queuing Time or Qt

Queuing Time is defined as the time spent waiting in a queue for access to computing resources. Queuing Time for a given business transaction can be also be defined as the End to End Queuing Time for access of any of the following physical resources i.e.

  * Queuing Time for access to Disk Resource
  * Queuing Time for access to CPU Resources
  * Queuing Time for access to Application Server Resources
  * Queuing Time for access to Database Server Resources

Lets revisit our basic equation for Response Time:

  * Rt = Wt + St &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;.  [ Wt = Wait Time, St = Service Time ]  **_also written as_**
  * Rt = Qt + St  &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;.  [ Wt = Wait Time, Qt = Queuing Time ]

Queuing Time [ Wt or Qt ] for a given application business transaction doesn't remain constant and is a variable that can change based on the congestion within the system and movement of congestion points within the given system. Longer queuing times will translate into more dropped connections and surely a lot more irate customers.

The Queue length for a given system or resource within a system can be calculated using the below formula:

  * <span style="font-family: Calibri;">Q = X * Qt </span><span style="font-family: Calibri;">  &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;..  </span><span style="font-family: Calibri;">[ X = Throughput, Qt = Queuing Time ]</span>

Performance Testing is generally conducted to identify potential system bottlenecks and understand the extent of queuing the system can take before the overall system performance starts degrading. Queuing on a system is inevitable and one can only invest that much of money to eliminate queuing based on choice of application designs and deployment architectures.


### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

