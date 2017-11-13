---
layout: pagelayout
title: What Is Service Demand
---

Let's start by taking a look at the definition of Service Demand.

Service Demand, Service Time and Visit Count are important metrics that describe system behavior and are used in analytical equations to model System Performance. Before we go ahead and define Service Demand we need to agree on the definition of Visit Count. So let&#8217;s start by taking a look at what Visit Count means in the context of System Performance.

### What Is Visit Count

(V) &#8211; Visit count is the count of the total number of service requests a given Entity (Request) makes at a given System Resource. Visit counts will vary from business transaction to transaction. For example: Visit count for Order Submit at the Application Server is 10 and at the Database Server is 15.

V<sub>app</sub> = 10, V<sub>db</sub> = 15

Visit Count simply speaking is the total number of visits made by every Entity at a given System Resource. A System Resource in this case could either be a whole application tier or a component within an application tier i.e. cpu, memory, disk, network, etc.

### What Is Service Demand

(D) &#8211; Service Demand is the total Service Time spent by a particular Entity at a given System Resource. As we have defined earlier, Service Time is simply the time taken to process a given Service Request. A System Resource in this case can be a computational resource, network resource, disk resource or a memory resource. A System Resource can also be a System Tier offering a particular application service which encapsulates computational, memory, disk, storage and network services behind it. Service Demand therefore depends on the total number of Visit Counts at a given System Resource.

Let us look at the System illustrated above. The image above depicts the following scenario:

  * Arrival of an Entity
  * Processing of the Entity by a System
  * Entity making a Service Request at 3 different System Components i.e. C<sub>1</sub>, C<sub>2</sub>, C<sub>3</sub>
  * Completion of the processing within the System and exit of the Entity from the System

The various system metrics we will need to consider are:

  * Component C<sub>1</sub>, Service Time (S<sub>1</sub>), Visit Count (V<sub>1</sub>), Service Demand (D<sub>1</sub>)
  * Component C<sub>2</sub>, Service Time (S<sub>2</sub>), Visit Count (V<sub>2</sub>), Service Demand (D<sub>2</sub>)
  * Component C<sub>3</sub>, Service Time (S<sub>3</sub>), Visit Count (V<sub>3</sub>), Service Demand (D<sub>3</sub>)

The System we are looking at has three main components C<sub>1</sub>, C<sub>2</sub> and C<sub>3</sub>. Each of these 3 components is load balanced internally and has 3 failover instances running. The Entity (Request) passing through the System makes requests at each of the various System Components C<sub>1</sub>, C<sub>2</sub> and C<sub>3</sub>. The Service Demand for the given Entity (Request) at the various System Components can be defined as:

  * D<sub>1</sub> = V<sub>1</sub> * S<sub>1</sub>&#8230;&#8230;&#8230;&#8230;.  [ Service Time (S<sub>1</sub>), Visit Count (V<sub>1</sub>), Service Demand (D<sub>1</sub>) ]
  * D<sub>2</sub> = V<sub>2</sub> * S<sub>2</sub>&#8230;&#8230;&#8230;&#8230;. [ Service Time (S<sub>2</sub>), Visit Count (V<sub>2</sub>), Service Demand (D<sub>2</sub>) ]
  * D<sub>3</sub> = V<sub>3</sub> * S<sub>3</sub> &#8230;&#8230;&#8230;&#8230;. [ Service Time (S<sub>3</sub>), Visit Count (V<sub>3</sub>), Service Demand (D<sub>3</sub>) ]

Also mathematically it can be proven that: X<sub>max</sub> <= 1/D<sub>max</sub>

The above equation basically tells us that the maximum System Throughput is Lesser than or Equal to the reciprocal of the maximum Service Demand.

Let&#8217;s look at application of the Service Demand concept using the following example:

**Example** &#8211; A business transaction issued by a user for the above system creates an Entity (Request) makes 10 requests at the first component with Service Time 3s, 15 requests at the second component with Service Time 4s and 20 requests at the third component with Service Time 5s. Determine the Service Demand at each of the System Components for the given Entity (Request). Also establish maximum system throughput.

  * D<sub>1</sub> = 10 * 3 = 30
  * D<sub>2</sub>= 15 * 4 = 60 <sub><br /> </sub>
  * D<sub>3</sub>= 20 * 5 = 100

Hence X<sub>max</sub> <= 1/100 <= 0.01. X<sub>max</sub> in this case is the maximum throughput that one can expect for the above system.

### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

