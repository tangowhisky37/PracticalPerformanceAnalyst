---
layout: pagelayout
title: What Is Universal Scalability Law
---

### What Is Universal Scalability Law

Dr. Neil Gunther put together the original derivation of Universal Scalability Law, or USL and presented it at the 1993 CMG conference. At the conference Dr. Gunther provided a brief account of its application to parallel processing performance (USL was previously called super-serial model). Dr. Gunther provided a more complete derivation of Universal Scalability Law with sample applications in Chaps. 4-6 of his GCaP (Guerrilla Capacity Planning) book. In Dr. Gunther&#8217;s words, here are some of the reasons why we should understand the Universal Scalability Law:

  * _A lot of people use the term &#8220;scalability&#8221; without clearly defining it, let alone defining it quantitatively._
  * _Computer system scalability must be quantified. If you can&#8217;t quantify it, you can&#8217;t guarantee it. The universal law of computational scaling provides that quantification._
  * _One of the greatest impediments to applying queueing-theory models (whether analytic or simulation) is the inscrutibility of service times within an application._
  * _Every queueing facility in a performance model requires a service time as an input parameter. Without the appropriate queues in the model, system performance metrics like throughtput and response time, cannot be predicted._
  * _The USL leapfrogs this entire problem by NOT requiring ANY low-level service time measurements as inputs._

Dr. Gunther&#8217;s Universal Scalability Law provides an understanding of system scalability as being made up of three different system characteristics i.e. Concurrency, Contention and Coherency. Through the models that Dr. Gunther put together he demonstrated how Universal Scalability Law can be used to understand and predict the behavior of any system.

To learn more about Universal Scalability Law please head to the Official page at <a href="http://www.perfdynamics.com/Manifesto/USLscalability.html" target="_blank">Dr. Gunther&#8217;s website</a>.

### Who Discovered Universal Scalability Law

Dr. Neil Gunther is an Australian of German and Scots ancestry, born in Melbourne on 15 August 1950. Dr. Neil Gunther, is a computer information systems researcher best known internationally for developing the open-source performance modeling software Pretty Damn Quick and developing the Guerrilla approach to computer capacity planning and performance analysis. He has also been cited for his contributions to the theory of large transients in computer systems and packet networks, and his universal law of computational scalability.

You can learn more about Dr. Gunther at <a href="https://en.wikipedia.org/wiki/Neil_J._Gunther" target="_blank">Wikipedia</a>.

### What Are The Equations for Universal Scalability Law

Universal Scalability Law defines a single scalability model that defines the relative capacity C(N) :

C(N) =  N / [1 + alpha (N - 1) + Beta N (N - 1) ]

The three terms in the denominator of the equation above are associated respectively with the three Cs we spoke about earlier:

  * The level of Concurrency or ideal parallelism: basically, linear scaling
  * The level of Contention (with strength alpha) due to waiting or queueing for shared resources
  * The level of Coherency (with strength beta) due to the delay for data to become consistent (or coherent) by virtue of point-to-point exchange

These parameter values are defined over the range: 0 <= alpha, beta <= 1. The independent variable N can represent either  concurrent users or processes.

To learn more about Universal Scalability Law please head to the Official page at <a href="http://www.perfdynamics.com/Manifesto/USLscalability.html" target="_blank">Dr. Gunther&#8217;s website</a>.


### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

