---
layout: pagelayout
title: What Is Littles Law
---

Little's law in many ways can be looked at as the foundation of performance. Little's Law helps us understand the reasons why systems bottleneck and provides a simple approach to understand concurrency or user in systems.

### Littles Law

John Dutton Conant Little, is an Institute Professor at the Massachusetts Institute of Technology, best known for his result in Operations Research, Littles Law. Littles law is truly amazing in its simplicity and can be used to describe the most complex of systems including resources within those systems.

![Queuing System]({{ "/assets/img/queuing_system.png" | absolute_url }})

Lets take for example the system described above. The notations used include:

  * N - Number of users present within the system
  * C - Number of completions
  * X - Throughput or Rate of Departure
  * A - Number of Arrivals
  * _Î»_ - Rate of Arrival
  * Rt - Time spent by Customers within the system

Littles Law basically states that the long-term average number of customers in a stable system _N_ is equal to the long-term average effective arrival rate, _Î»_, multiplied by the average time a customer spends in the system, W or Rt, or expressed algebraically:

  * N = _Î»_ * Rt &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;..  [ N = Number of Users in the System, Rt = Response Time, _Î»_ = Arrival Rate ]

Littles Law can also be stated as:

  * N = Rt * X &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;..  [ N = Number of Users in the System, Rt = Response Time, X = Throughput ]

For a system where Zt (Think Time is Non Zero) Littles Law can be stated as:

  * N = [Rt + Zt] * X  &#8230;&#8230;&#8230;&#8230;&#8230;&#8230;..  [ N = Number of Users in the System, Rt = Response Time, Zt = Think Time, X = Throughput ]

<p style="text-align: left;" align="center">
  <strong>Applying Little&#8217;s Law: </strong> Now that we have just defined Littles Law lets take a look at where we could apply Littles Law and benefit from a better understanding of our systems including user behavior on our existing systems.
</p>

Littles Law can be applied to the following scenarios:

![Queuing Systems In Real Life]({{ "/assets/img/line_at_starbucks.png" | absolute_url }})

  * Model Performance Testing Workload
  * Validate Performance Testing Results
  * Validate the Sizing Models that your Infrastructure guys have come up with
  * Validate the Non Functional Requirements that your Architects have recommended

Lets take a look at a few examples and apply Littles Law to a real world system:

**Example - Determine Concurrent Users Using Littles Law:** A system at peak processes 8000 Transactions/Hour with an average response time of ~5s per transaction. The average Think Time per user is ~30s. What is the number of concurrent users on the system?

  * Throughput or X = 8000/3600 = 2.22 TPS
  * We know: N =  [Rt + Zt] * X  &#8230;&#8230;&#8230;.. [ N = Number of Users in the System, Rt = Response Time, Zt = Think Time, X = Throughput ]
  * Applying the equation: N = [ Rt + Z ] \* X = [ 5 + 30 ] \* 2.22 = 77.7
  * The above system has approximately 77 users at peak driving 8000 Transactions/Hour.

**Example - Validate System Performance Testing Results:** The outcome of a performance test is as follows:

  * Peak User Concurrency = 1000
  * Average Transactional Response Time = 5s
  * Average User Think Time = 40s
  * Peak Transactional Throughput ( as recorded by the tool) = 500 TPS

We know: N =  [Rt + Zt] * X  &#8230;&#8230;&#8230;..  [ N = Number of Users in the System, Rt = Response Time, Zt = Think Time, X = Throughput ]

  * Applying the equation:  X = N / [ Rt + Z ] = 1000 / [ 5 + 40 ] = 22.22 TPS

You know from the above results, something is really wrong. Littles Law suggests that the actual TPS for the above system should be ~22 TPS but the Performance Testing results show transactional throughput as 500 TPS. Could this be errors in the Performance Testing results due to poorly written scripts? If your scripts are not smart enough to catch all the relevant errors, the Performance Testing tool will include the errors as part of the true transactional throughput.

The above two examples are meant to give you some familiarity with Littles Law and help you apply Littles Law to model Performance Testing workload including validating your Performance Testing results.


### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

