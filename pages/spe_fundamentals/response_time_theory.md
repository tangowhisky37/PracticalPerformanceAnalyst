---
layout: pagelayout
title: What Is Response Time Theory
---

Let's start by defining what we mean by a Response Time model.

### Response Time Model

The Response Time model is a simple way of calculating the overall Queue Length and Queuing Time for a given system for a given set of workload conditions. The Response time Model is generally used for back of the envelope calculations and to get a sense of direction. We wouldn't recommend using Response Time models to make investment or major architectural design decisions. For more detailed performance modelling when validating architectural decisions or investment decisions we would recommend investing in building thorough Queuing Theory models.

To be able to use the Response Time model at minimum you would need to know two of the three variables mentioned below:

  * Uavg - Average System Utilization
  * X  - System Throughput
  * St - Service Time

M is always assumed to be known since it's the number of CPU's (also called Servers when referring to performance models) within the system. This is a design assumption and is assumed to be a known quantity.

  * M - Number of Servers

Let's take a look at all of the equations and then look at a real world example:

  * U<sub>avg</sub> = [ X * S<sub>t</sub> ] / M &#8230;&#8230;&#8230;&#8230;&#8230;..  [ U<sub>avg</sub> = Average Utilization,  X = Throughput, S<sub>t</sub> = Service Time, M = Number of Servers ]
  * R<sub>t-cpu</sub> = St / [ 1 &#8211;  (U<sub>avg)</sub><sup>M</sup> ]&#8230;&#8230;&#8230;..  [ Rt = CPU Response Time, U<sub>avg</sub> = Average Utilization,  S<sub>t</sub> = Service Time, M = Number of Servers ]
  * R<sub>t</sub> = Q<sub>t</sub> + S<sub>t</sub> &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;..  [ S<sub>t</sub> = Service Time, R<sub>t</sub> = Response Time, Q<sub>t</sub> = Queuing Time ]
  * Q<sub>t</sub> = R<sub>t</sub> &#8211; S<sub>t</sub>&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;  [ R<sub>t</sub> = CPU Response Time, Q<sub>t</sub> = Queuing Time, S<sub>t</sub>= Service Time ]
  * Q = X * Q<sub>t</sub> &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;&#8230;..  [ Q = Queue Length, Q<sub>t</sub> = Queuing Time, S<sub>t</sub> = Service Time ]

**Example:** The best way to understand these laws is to look at an example and work our way through the various equations:

Lets assume we observe a system with 4 CPUs for a period of 1 Hour or 3600 seconds out of which the system has been busy for 1000 seconds. For the duration of observation there were 500 successfully completed transactions. Lets use the very basic Response Time theory to do some quick back of the envelope transactions and understand what the Queuing Times would be and how long would the Queue have been on the system.

  * T = 3600 seconds [ Total Time of Observation ]
  * B = 1000 seconds [ Busy Time ]
  * C = 500  [ Completions ]
  * M = 4 [ Number of CPUs or Servers ]

  * We know from our fundamental equations : <ul style="list-style-type: circle;">
      <li>
        <strong>St = B / C </strong>.........[ St = Service Time, B = Busy Time, C = Completions ]
      </li>
      <li>
        Therefore : St = 1000 / 500 = 2 seconds
      </li>
    </ul>

  * We also know from our fundamental equations: <ul style="list-style-type: circle;">
      <li>
        <strong>X = C / T </strong>...........[ X = Throughput, C = Completions, T = Total Time of Observation ]
      </li>
      <li>
        X = 500 / 3600 = 0.139 TPS
      </li>
    </ul>

  * We also know:
      * **U<sub>avg</sub> = [ X * S<sub>t</sub>]** .........[ Uavg = Average Utilization ]
      * Uavg = [ 0.139 * 2 ] / 4 = 0.0695
      * The Average Utilization Per Processor is 0.0695

  * We also know :
      * **Rt = S<sub>t</sub> / [ 1 - (U<sub>avg</sub>)<sup>M</sup> ]** ....... [ Rt = CPU Response Time ]
      * Rt = 2 / [ 1 - (0.0695)<sup>4</sup>]
      * Rt = 2 / [ 1 - 0.00002 ]
      * Rt = 2.000 seconds

  * We also know:
      * **R<sub>t</sub> = Q<sub>t</sub> + S<sub>t</sub>** .......[ Qt = Queuing Time ]
      * Qt = Rt - St
      * Qt = 2.0 - 2.0  [ St = 2s, Rt = 2.0s)
      * Qt = 0 seconds

  * We also know: <ul style="list-style-type: circle;">
      <li>
        <strong>Q = X * Q<sub>t</sub></strong> [ Q = Queue Length ]
      </li>
      <li>
        Q = 0.139 * 0
      </li>
      <li>
        Q = 0
      </li>
    </ul>

Thus, using Response Time theory we have figured out that the actual Queue size Per CPU is 0 for the above set of variables.

We hope this example has illustrated the simplicity and power of Response Time Theory to estimate potential system bottlenecks. As we have mentioned before, only use Response Time models for quick back of the envelope calculations when you need to get a gut feel and direction. For a more detailed system performance model we would encourage you to consider using Erlang C model or Queuing Theory models which we have covered in other sections.


### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

