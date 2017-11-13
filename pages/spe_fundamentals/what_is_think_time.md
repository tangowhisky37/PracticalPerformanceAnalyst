---
layout: pagelayout
title: What Is Think Time
---

Let's start by taking a look at the definition of Think Time -

### Think Time or Zt

Applications are generally built to automate business processes and each business process could be viewed as a collection of numerous simple user actions that are strewn together to achieve a certain objective. Unlike robots users rarely perform such actions repeatedly or in succession one after the other without pausing for thought or performing some action required to provide the application input. 

Users generally tend to perform actions in repeated sequence with varying amounts of time between them depending on the complexity of the relevant user action i.e. the action of filling up a simple form could vary from 10-30s before the user hits the submit button.

Think Time is thus defined as the time taken by a user between two consecutive actions and is generally represented by the letter Z. Think Time is usually measured in terms of seconds and is represented as follows : **Z** = 30s

![Concept of Think Time]({{ "/assets/img/concept_of_think_time.png" | absolute_url }})

Think Time plays a very important role in Performance Engineering including on-going Performance & Capacity Management of any system. Without a good understanding of your users Think Time you can end up building un-realistic Performance Models required to simulate system performance or even end up building Workload Models for Performance Test which could impose higher than expected workload on your systems. Lets see how accuracy of Think Time can affect the outcome of a simple performance test:

  * **Real value of Z = 30 seconds**

  * **Incorrectly Assumed value of Z = 5 seconds** - In this case the Performance Testing Workload Models you build will end up performing actions and eventually business transactions at a higher rate than what the system in production would actually be handling. As a result the system in Performance Test is going to be forced to handle a lot more workload that it actually would in a normal production scenario.

  * **Incorrectly Assumed value of Z = 60 seconds** - In this case the Performance Testing Workload Models you build would end up performing actions and eventually business transactions at a much lower rate than what the system in production would be eventually handling. As a result the system in Performance Test isnt going to be stressed hard enough and you wouldnt have a true understanding of what the real end user performance is going to look like.

In general during Performance Test one sets up the run settings such that Think Time (Z) is varied between a set of given constants. This is to introduce variability mimicking the nature of different clients accessing the applications. Thus an accurate understanding of Think Time for each of the critical business processes is essential for you as the Performance Engineer to accurately simulate Workload Models during Performance Test, Modelling application performance during Architecture/Design or Predicting Capacity impacts at go live.

### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

