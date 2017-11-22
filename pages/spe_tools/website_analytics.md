---
layout: pagelayout
title: Tools - Website Analytics
---

### What is Web Analytics (Web Log Analysis)

Web Log Analysis is the process concerned with the collection, measurement, analysis & reporting of user traffic insights for the purpose of understanding the workload across the website. In short Web Log Analysis is about gathering comprehensive data on end user access patterns, access times, traffic insights of customers/users accessing the system from different parts of the world, navigation pattern across the application, typical session duration, browsers used, platform used, etc. Web Log Analysis helps with obtaining a strong understanding of the usage profile of the entire web application. The web application could be an internally hosted application or an externally hosted application i.e. hosted on the internet for anyone to access. 

Web site analytics is a key activity that can provide metrics required to understand traffic patterns, current system performance, end user behaviour, hotspots across the application which receive the most amount of hits, application components that generate the most amount of errors, user demand with regards to times of day when peaks and troughs (user access) occurs, etc. All of these metrics are key to build a workload model which you can then use as an input into performance testing, performance modelling and capacity management. 

### Analysis of Web Site Statistics 

There are two main methods for performing website analytics - Web log file analysis and Script-based analysis. Every time a user visits a website, the web server has the ability to record all the relevant information about the user access request. This typically includes the time of access, types of files accessed & downloaded, browser used, operating system used, geographic location, IP address, bandwidth used, referring websites, HTTP response codes, Page Views, page processing time, search spiders, etc. All of this data is generally stored by the web server in a log files. **Web log analyzers** can then be used to interpret the data stored within the log files to obtain meaningful insights & stores them in a database to generate reports on demand. There are a few different Web Log File formats but some of the most common ones are - 

* Apache log file formats like NCSA combined/XLF/ELF log format or common/CLF log format 
* IIS log file format like W3C log format, etc.

Alternatively, **Script based analyzers** use a JavaScript based tracking code to be added on every webpage in the website that needs to be included in the web analytics. This tracking code places a cookie on the visitor's computer/device to track the webpage usage & captures the user access details. Java Script based analyzers e.g. Google Analytics, sends data for all of the metrics (outlined above) to a remote server generally in an asynchronous fashion ( to avoid penalizing end user performance).

### Challenges Using Web Site Analytics

It's possible that the traffic data reported by Log Analyzer tools are higher as they process the log file data from Web server which tracks every user interaction with the website whereas Script based Analyzers record data from pages that have JavaScript tracking enabled & captures user details who use cookie/JavaScript enabled browsers (so they rarely track 100% of visitors). There's no right or wrong way or obtaining Web Site Usage statistics. We would recommend using a combination of the above techniques.

<div class="table-responsive">
  <table  style="width:600px; "  class="easy-table easy-table-default " border="0">
    <tr>
      <th  style="width:150px;text-align:left" >
        Vendor
      </th>

      <th  style="width:100px;text-align:left" >
        Area Of Focus
      </th>

      <th  style="width:150px;text-align:left" >
        Free
      </th>

      <th  style="width:100px;text-align:left" >
        Link
      </th>
    </tr>

    <tr>
      <td  style="text-align:left" >
        AWStats
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://www.awstats.org/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        W3Perl
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://www.w3perl.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Splunk
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.splunk.com" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Kibana/Logstash
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="https://www.elastic.co/products/kibana" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Go Access
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="https://www.elastic.co/products/kibana" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Webalizer
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://www.webalizer.org/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        IIS Log Parser
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="https://gallery.technet.microsoft.com/office/Log-Parser-Studio-cd458765" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Apache Log Viewer
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.apacheviewer.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Deep Log Analzyer
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.apacheviewer.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Apache Log Analzyer
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Shareware
      </td>

      <td  style="text-align:left" >
        <a href="http://www.brothersoft.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Web Log Expert
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://weblogexpert.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Alterwind
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.alterwind.com/loganalyzer/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Nihuo
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.loganalyzer.net/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Visitors
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://www.hping.org/visitors/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Sawmill
      </td>

      <td  style="text-align:left" >
        Web Log Analyzer
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.sawmill.net" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Piwik
      </td>

      <td  style="text-align:left" >
        Javascript/PHP PageTag
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://piwik.org" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        CrawlTrack
      </td>

      <td  style="text-align:left" >
        PHP PageTag
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://www.crawltrack.net/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Piwik
      </td>

      <td  style="text-align:left" >
        Javascript/PHP PageTag
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://piwik.org" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Google Analytics
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.google.com/analytics" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        WebTrends
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.webtrends.com" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Adobe
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.adobe.com/in/marketing-cloud/web-analytics.html" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Mint
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.haveamint.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        SiteMeter
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.sitemeter.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        StatCounter
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://statcounter.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Web Trek
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="https://www.webtrekk.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Map My User
      </td>

      <td  style="text-align:left" >
        Javascript
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://www.mapmyuser.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Real Tracker
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.realtracker.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Power Phlogger
      </td>

      <td  style="text-align:left" >
        Javascript/Cookie
      </td>

      <td  style="text-align:left" >
        Free
      </td>

      <td  style="text-align:left" >
        <a href="http://pphlogger.phpee.com/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
        Smarter Stats
      </td>

      <td  style="text-align:left" >
        Self-Hosted/Web Log File
      </td>

      <td  style="text-align:left" >
        Free/Commercial
      </td>

      <td  style="text-align:left" >
        <a href="http://www.smartertools.com/smarterstats/" target="_blank">Link</a>
      </td>
    </tr>

    <tr>
      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>

      <td  style="text-align:left" >
      </td>
    </tr>
  </table>
</div>

Hope you've enjoyed the content in this section at Practical Performance Analyst and have learnt something new. Please help us grow the community by taking a moment and sharing this content with rest of community using your preferred Social Media Platform (links provided below). We are looking for the bright spark and if you think you have what it takes to build and grow this community reach out to me by [Sending us an email](mailto:elearning@practicalperformanceanalyst.com?subject=Feedback%20).
