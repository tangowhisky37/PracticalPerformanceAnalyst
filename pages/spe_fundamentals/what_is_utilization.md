---
layout: pagelayout
title: What Is Utilization
---

Let's start by taking a look at the definition of Utilization. 

### Utilization or U

Utilization of any system is defined as the Ratio of Busy Time to Total Time of Observation. Utilization is a ratio that generally refers to how busy or free the resources within a given system are. Utilization can also be used to refer to how busy or free are components within a given system instead of the system as a whole.

The following equations are used to describe Utilization:

  * U = Bt / T   &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;. [ Bt = Busy Time, T = Total Observed Time Interval ]

The above equation describes utilization as the ratio of Busy Time to Total Observed Time.

**Example:** Lets assume we are viewing a system for a period of 180 seconds during which it remains busy for 100 seconds.

  * The Utilization of the system is calculated as follows:
  * We know : U = Bt / T   &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;. [ Bt = Busy Time, T = Total Observed Time Interval ]
  * Utilization (U) = 100/180 = 0.55

The Utilization thus for this system is 0.55.

In addition to the equation above Utilization can be described as:

  * U = X * St   &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;. [ X = Throughput, St = Service Time ]

The above equation describes Utilization as the product of Throughput and Service Time. As mentioned earlier the above equation can be applied to either the system as a whole or at a resource level within a given system.

**Example:** Lets assume we are viewing a system for a period of 180 seconds during which it remains busy for 100 seconds. The Service Time for a transaction is 2s. The throughput of the system is calculated as follows:

  * U = X * St
  * X = U / St = 0.55 / 2 = 0.275 Transactions/Sec

The equation provided below is very similar to the previous equation but with one subtle difference i.e. the addition of Average Number of Servers (of CPU&#8217;s in our case).

  * U<sub>avg</sub> =Â  [ X * St ] / M &#8230;&#8230;&#8230;&#8230;&#8230;.. [ U<sub>avg</sub> = Average Utilization, X = Throughput, St = Service Time, M = Average Number of Servers  ]

On a system with multiple servers (CPUs) the average utilization is obtained by dividing the overall system utilization by the total number of servers (CPUs) present.


### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

