---
layout: pagelayout
title: What Is Time To First Buffer
---

### Time to First Byte or TTFB

Another important Performance Quantity associated with Response Time is &#8211; **Time To First Byte** or **TTFB** in short. Time To First Byte is the Elapsed Time between submission of the request and receipt of the first response from the server. TTFB like Response Times can be measured either at the Application Tier level or within an Application Tier at any of system components i.e. CPU, Memory, Disk, Network, etc.

The Time To First Buffer is an indication of how heavy the processing for a given workload is or even an indication of how long does it take to open up a connection to a particular resource for the first time due to various buffering requirements. Time to First Buffer is used a lot by Performance Testing teams and is also used to optimize the way applications deliver their payload to customers. Time To First Buffer gains a lot of relevance with applications where the rendering times are significant.

![Time To First Buffer]({{ "/assets/img/time_to_first_buffer.png" | absolute_url }})

Let&#8217;s take a look at an example to understand the relevance of Time To First Buffer.

**Example:** Let&#8217;s say the user has submitted an Order Submit request at time t=0s. Let&#8217;s assume that the overall response time for the transaction is 10s, but the client received the first response at t=5s while rest of the time is actually spent by the client GUI engine rendering the payload on the client machine while still receiving the rest of the payload from the server.

A large Time To First Buffer should be a cause of concern. From experience large TTFB could be due to any of the following reasons:

  * Lack of DNS caching
  * Poor caching of application objects
  * Poor or lack of caching of web objects
  * Poor links connection clients and servers
  * Challenges with the load balancing and networking setup causing delayed connections
  * Challenges with application performance delaying allocation of resources to initiate connections

### Additional Resources

* [Dr. Rajesh’s papers on Performance Testing and Performance Requirements Gathering](https://sites.google.com/site/swperfengg/)
* [Microsoft : Load Testing of Web Applications](http://msdn.microsoft.com/en-us/library/bb924372.aspx)
* [Microsoft : Patterns & Practices – Performance Testing Guidance](http://perftesting.codeplex.com/wikipage?title=How%20To:%20Model%20the%20Workload%20for%20Web%20Applications)
* [The Server Side : Performance Engineering – A Practitioners approach to Performance Testing](http://www.theserverside.com/news/1363731/Performance-Engineering-a-Practitioners-Approach-to-Performance-Testing)
* [Dr. Connie Smith on Performance Engineering](http://www.perfeng.com)
* [Dr. Rajesh Mansharamani on Performance Engineerirng](https://sites.google.com/site/swperfengg/home)
* [Wikipedia on Performance Engineering](http://en.wikipedia.org/wiki/Performance_engineering)

Hope you’ve enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by Sending us an email. 

