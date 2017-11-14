---
layout: pagelayout
title: What Is Queuing Theory
---

### What does Wikipedia say about Queueing Theory

According to Wikipedia Queueing Theory can be defined as, “The mathematical study of waiting lines, or queues. In queueing theory a model is constructed so that queue lengths and waiting time can be predicted. Queueing theory is generally considered a branch of operations research because the results are often used when making business decisions about the resources needed to provide a service. Queueing theory has its origins in research by Agner Krarup Erlang when he created models to describe the Copenhagen telephone exchange. The ideas have since seen applications including telecommunication, traffic engineering, computing and the design of factories, shops, offices and hospitals.

Agner Krarup Erlang, a Danish engineer who worked for the Copenhagen Telephone Exchange, published the first paper on what would now be called queueing theory in 1909. He modeled the number of telephone calls arriving at an exchange by a Poisson process and solved the M/D/1 queue in 1917 and M/D/k queueing model in 1920. In Kendall’s notation:

* M stands for Markov or memoryless and means arrivals occur according to a Poisson process
* D stands for deterministic and means jobs arriving at the queue require a fixed amount of service
* k describes the number of servers at the queueing node (k = 1, 2,…). If there are more jobs at the node than there are servers then jobs will queue and wait for service“

You can read more about the basics of Queueing Theory at Wikipedia [Link](https://en.wikipedia.org/wiki/Queueing_theory).

### Why Do We Need Queueing Theory

As any system gets congested or loaded a queue of sorts starts to build up. This build up of congestion could apply to components within the system and also the system as a whole with queueing building up externally. A good understanding of the service times, the queueing times and the relationship of workload (increase and decrease) is essential to understanding the principles underpinning Queueing Theory. Queueing is part of our every day life i.e. from queueing at ATMs to withdraw money to waiting to be served at the counter when purchasing your cup of freshly brewed coffee every morning. We don&#8217;t generally realize how life around us plays out as a system of systems with Queueing Theory applicable to most of them.

Lets now focus on compute infrastructure which is a very common application of Queueing Theory for Systems Performance Engineers. There are various reasons why you need to understand the basics of Queueing Theory here.

  * Like every system any information technology system has limited resources
  * Every system provides certain functionality and does so with a given set of service times
  * As the workload processed by the system goes up the utilization levels of the system go up and queueing at the various resources gradually starts to build up
  * An increase in queueing does not change the service time for the system but rather increases the amount of wait time at a given resource
  * The increase in workload causes building up of queues outside the system and potentially at various key resource blocks across the system (depending on how the system is designed)
  * A perceived increase in response time is noted. This includes a constant &#8220;Service Time&#8221; and a variable &#8220;Wait Time&#8221;

### So What Do We Do With All This Queueing Models

Thus as you have noted above an understanding of Queueing Theory helps Systems Performance Engineers understand how an increase in user workload within a system can cause an increase in customer wait times and hence overall perceived response times. Armed with this information the System Performance Engineer can do a few things. He or she can:

  * Tune the system bottlenecks so as to increase transactional throughput and hence delay the impact of queues
  * Impact the system configuration by increasing the amount of compute resources available for processing. This again will change the behavior of the system
  * Impact the way the users access the system and prioritize user requests. This allows for processing of higher prioritized user requests first followed by the lower priority ones.
  * Provide a pool of resources for the system to consume so that an increase in workload triggers an increase in compute resources and avoids building up of queues

There are various ways a Performance Engineer could impact the design of a system with a solid understanding of queues.

### Kendalls Notation for Queueing Theory

Before we look into the various Queueing Theory equations let us go over the notation system designed by Kendall to describe a Queueing system.

Let us denote a system by A / B / m / K / n/ D, where

  * A: distribution function of the inter-arrival times,
  * B: distribution function of the service times,
  * m: number of servers,
  * K: capacity of the system, the maximum number of customers in the system including the one being serviced,
  * n: population size, number of sources of customers,
  * D: service discipline.

Exponentially distributed random variables are notated by M, meaning Markovain or memoryless. Furthermore, if the population size and the capacity is infinite, the service discipline is FIFO (First In First Out), then they are omitted.

Hence M/M/1 denotes a system with Poisson arrivals, exponentially distributed service times and a single server. M/G/m denotes an m-server system with Poisson arrivals and generally distributed service times. M/M/r/K/n stands for a system where the customers arrive from a finite-source with n elements where they stay for an exponentially distributed time, the service times are exponentially distributed, the service is carried out according to the requests arrival by r severs, and the system capacity is K.

Kendall&#8217;s equations are generally used to describe Queueing Systems making it easy to convey the system configuration using a single equation.

### Queueing Theory Equations

Here is a summary of the various key Queueing Theory equations:

  * U = (S<sub>t</sub> * X )/M &#8230;[U = System Utilization, S<sub>t</sub> = Service Time, X = Throughput, M = No Of Servers/CPU&#8217;s]
  * Q<sub>l</sub> = _L_ Q &#8230; [Q = Queueing Time, Q<sub>l</sub>= Queue Length, _L_ = Arrival Rate]
  * R<sub>t-cpu </sub>(For CPU Systems) = S<sub>t</sub> / [1-U<sup>m</sup>] &#8230;[R<sub>t-cpu</sub>=CPU Response Time, S<sub>t</sub>=Service Time, U = System Utilization, M = No Of Servers/CPU&#8217;s]
  * R<sub>t-io </sub>(For IO Systems) = S<sub>t</sub> / [1-U] &#8230;[R<sub>t-io</sub>=IO Response Time, S<sub>t</sub>=Service Time, U = System Utilization]
  * R<sub>t</sub> = S<sub>t</sub> + Q<sub>t &#8230; </sub>[ Rt = Response Time, St=Service Time]
  * _L_<sub>q</sub> = _L_<sub>sys</sub> / Q<sub>n</sub> &#8230; [ _L_<sub>q</sub> = Arrival Rate Per Queue, _L_<sub>sys</sub> = Total Arrival Rate for the System, Q<sub>n</sub> = Number of Queues  ]
  * Ec = ErlangC (m, St, _L_q) = [ (M S<sub>t </sub>_L_<sub>q</sub>)<sup>m </sup>/ M! ] / [ (1 &#8211; m S<sub>t</sub>) Sigma<sub>K=0</sub><sup>M=1</sup> [ ((m S<sub>t </sub>_L_<sub>q</sub>)<sup>K</sup> / K! ) + ] ((m S<sub>t </sub>_L_<sub>q</sub>)<sup>M</sup> / M! ) ]

The above equations have probably made your head spin a bit and I wouldn&#8217;t blame you for that. Not being a mathematician myself it took me a while to piece together the whole picture and work out how to best use the above equations to model performance of the system for increases in workload. For those who want to avoid creating complex models using error prone excel see the option provided below.

### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

