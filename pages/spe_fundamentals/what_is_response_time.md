---
layout: pagelayout
title: What Is Response Time
---

Let's start by taking a look at the definition of Response Time. 

**Defining Response Time** (**Rt)** &#8211; Response Time is one of the most fundamental quantities in Performance Engineering. Response Time is defined as the Total Elapsed time between submission of a request and receipt of the response. Response Times can be measured at different tiers for a given application i.e. Web Server Response Time, Application Server ResponseÂ Time, Database Server Response Time, etc. Response Times can also be measured within a given tier across the various system components i.e. CPU Response Time, Memory Access Response, Disk Access Response Time, Network Transfer Response Time, etc. Â Response Times have traditionally been measured for critical business transactions during a performance test using Diagnostics tools or Performance Testing tools. Response Times can also be measured for Single User Performance Tests using plugins like Firebug on Firefox.

However, Response Times by-itself mean very little and do not provide anyone a good view of what the system performance looks like. One has to look at Response Times in conjunction with other Performance Quantities i.e. System Utilization, User Concurrency, Application Throughput, Network Bandwidth Utilization, expected System SLAâ€™s, etc. to understand what the true picture of Performance really is while keeping mind the cost of achieving that performance. Now that we&#8217;ve introduced the concept of Response Time let&#8217;s take the next step and see what the different types of Response Times are and where are these different Response Times measured.

Remember, Performance Engineering requires a holistic view of Performance for a given system.

The basic Response Time Equations are written as:

  * Rt = Wt + St &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;.Â  [ Wt = Wait Time, St = Service Time ]Â  **_also written as_**
  * Rt = Qt + StÂ  &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;.Â  [ Wt = Wait Time, Qt = Queuing Time ]

**Challenges Capturing Response Times &#8211;** Applications these days are quite complex and consist of complex workloads (i.e. Multiple transaction types with different transaction rates) and interact with numerous different internal and external application components using Web Services/SOAP or custom protocols.Â  MeasuringÂ Response Times for such applications has traditionally been easy at the Business Transaction level using standard Performance Testing tools.

But when it comes to measuring similar Response at each of the various application tiers (i.e. Web Server Tier, Application Server Tier, Database Server Tier, etc.) you run into challenges and things get further complicated if you need to capture response times for each of the workload components at the various systems components i.e. Response Time of the Order Submit Transaction at the CPU of the Application Server, Response Time of the Order Submit Transaction at the Disk Subsystem for Database Server.

  * End User Response Time = Web Server + App Server + EAI Server + DB Server OR
  * End User Response Time = (Rweb + Wweb) + (Rapp + Wapp) + (Reai + Weai) +( Rdb + Wdb)Â  &#8230;&#8230;..[W = Waiting Time]

Now one can further break down response time at any tier as demonstrated below:

  * Total Web Server Response Time = Time spent Queuing at Disk + Time spent on Disk IOPS + Time spent Queuing for CPU + Time spent at CPU
  * Total App Server Response Time = Time spent Queuing at Disk + Time spent on Disk IOPS + Time spent Queuing for CPU + Time spent at CPU
  * Total EAI Server Response Time = Time spent Queuing at Disk + Time spent on Disk IOPS + Time spent Queuing for CPU + Time spent at CPU
  * Total DB Server Response Time = Time spent Queuing at Disk + Time spent on Disk IOPS + Time spent Queuing for CPU + Time spent at CPU

The point we are trying to make here is that **Rt** can be abstracted down to any level depending on the nature of the performance problem you are trying to solve. If all you are concerned about is the overall End User Performance for a given transaction you donâ€™t have to go about measuring time spent by the transaction at each of the 10 Disks across the storage subsystem.

Measuring Response Times externally at the Business Transaction Tier using off the shelf Performance Testing tools or just a simple browser plugin like Firebug works really well. But when it comes to measuring Response Times for the Web Server Tier, Application Server Tier or the Database Server tier things get really complicated. This is simply because todays Performance Testing tools do not have the ability to go into the application and collect Response Times for each of the tiers. You could use traditional Diagnostics tools which sit inside the Application Container (.Net or Java) to capture response times across the various tiers but that wouldn&#8217;t completely solve the problem either because Diagnostics tools only work on Application Servers i.e. .Net and Java, they don&#8217;t all necessarily work with Web Servers and other proprietary applications that you might be connecting to. So while Diagnostics tools can give you an idea of the Response Times of each of the individual method calls between the Application Server and Database Server you won&#8217;t be able to correlate the Response Times across the various external application tiers and definitely not with the Performance Testing tool.

**Potential Solutions to Capturing detailed Tier wise Response Times &#8211;** There are a few solutions to the problem. One is to use transaction tracing tools that stamp packets with a code as the flow through the network. These agents sitting on the various servers (Web, Application, Database, etc.) need to have a good understanding of the application protocol along with support for the Operating System. The transaction tracing tool will then collect these statistics across the Web Servers, Application Servers, Database Servers, Messaging Servers, Web Services Servers, etc. and send them back to a central host that will provide an view of the Response Times across the various tiers. But try correlating this information with the results from the Performance Test and you&#8217;ll hit another brick wall. The second solution is to simply timestamp the message as it flows through the stack. The challenge with this approach is the fact that time stamping code takes time and very often you won&#8217;t have access to the source code of all the applications that you need to performance test.

Some of the newer Diagnostics tools i.e. New Relic and AppDynamics are changing the game and provide good view of End to End view of response times from the App Server through the Messaging Bus down to the Database server and even other 3<sup>rd</sup> Party applications.

### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

