---
layout: pagelayout
title: What Is Throughput
---

Let's start by taking a look at the definition of Response Time. 

### Throughput or X

Throughput is defined as the rate of completions for a given system. Its also defined as the total completions per unit time e.g. Transactions/Sec.

The equation for throughput is defined as:

<p align="center">
  <ul>
    <li>
      X = C / T ...............[C = Completions in time T, T = Total time of observation]
    </li>
  </ul>
  
  <p>
    <strong>Example: </strong>Lets assume we observe a system for a period of 180 seconds (3 minutes) during which there are 5 customers who successfully exit the system. The system can be described as:
  </p>
  
  <ul>
    <li>
      Completions or C = 5
    </li>
    <li>
      Time Period of Observation or T = 180s
    </li>
    <li>
      Throughput or X = C / T = 5 / 180 = 0.03 Transactions/Sec
    </li>
  </ul>
  
  <p>
    There is also one other interesting relationship between Maximum Throughput of a system and the Average Value of Service Time. Itâ€™s denoted by the following equation:
  </p>
  
  <ul>
    <li>
      Xmax <= 1 / Stavg........[Xmax= Max Value of Throughput possible, Stavg = Avg Value of Service Time ]
    </li>
  </ul>
  
  <p>
    The above equation is one of the most fundamental and important equations with regards to system performance, also called the bottleneck equation. The bottleneck equation basically states that the Maximum Throughput is inversely proportional to the Average (System/Component) Service Time. Using the above equation you can key in the Average Service Time for your bottleneck resource (resource or component within the system that has the highest Service Time) within your system and obtain the maximum possible throughput the system can achieve.
  </p>
  
  <p>
    <strong>Example: </strong>Lets assume for the same system above the poorest performing component has a Service Time of 3s i.e. This is the component within the system with the largest Service Time.
  </p>
  
  <p>
    Thus Xmax <= 1/3s = 0.33 Transactions/Sec. This particular system can never achieve a throughput more than 0.33 Transactions/Sec as long as the largest Service time within the system is 3s.
  </p>
  
  <p>
    The above equation comes in very handy when validating performance testing results. The bottleneck equation is also very frequently used to perform back of the envelope calculations for bottleneck and throughput analysis.
  </p>
</p>


### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

