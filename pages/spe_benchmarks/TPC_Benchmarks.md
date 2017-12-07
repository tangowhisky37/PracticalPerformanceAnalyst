---
layout: pagelayout
title: TPC Benchmarks
---

### TPC-C (Source : tpc.org) 

TPC-C simulates a complete computing environment where a population of users executes transactions against a database. The benchmark is centered around the principal activities (transactions) of an order-entry environment. These transactions include entering and delivering orders, recording payments, checking the status of orders, and monitoring the level of stock at the warehouses. While the benchmark portrays the activity of a wholesale supplier, TPC-C is not limited to the activity of any particular business segment, but, rather represents any industry that must manage, sell, or distribute a product or service.

TPC-C involves a mix of five concurrent transactions of different types and complexity either executed on-line or queued for deferred execution. It does so by exercising a breadth of system components associated with such environments, which are characterized by:

<ul class="squareblk">
  <li>
    The simultaneous execution of multiple transaction types that span a breadth of complexity
  </li>
  <li>
    On-line and deferred transaction execution modes
  </li>
  <li>
    Multiple on-line terminal sessions</li>
  <li>
    Moderate system and application execution time
  </li>
  <li>
    Significant disk input/output
  </li>
  <li>
    Transaction integrity (ACID properties)
  </li>
  <li>
    Non-uniform distribution of data access through primary and secondary keys
  </li>
  <li>
    Databases consisting of many tables with a wide variety of sizes, attributes, and relationships
  </li>
  <li>
    Contention on data access and update
  </li>
</ul>

TPC-C performance is measured in new-order transactions per minute. The primary metrics are the transaction rate (tpmC), the associated price per transaction ($/tpmC), and the availability date of the priced configuration.

To see additional benchmark details and results please <a href="http://www.tpc.org/tpcc/results/tpcc_results.asp?orderby=hardware" target="_blank">Click Here</a>.

### TPC-DS (Source : tpc.org)  

TPC-DS is TPC's decision support benchmark that models several generally applicable aspects of a decision support system, including queries and data maintenance. Although the underlying business model of TPC-DS is a retail product supplier, the database schema, data population, queries, data maintenance model and implementation rules have been designed to be broadly representative of modern decision support systems. This benchmark illustrates decision support systems that:

<ul class="BodyText">
  <li>
    Examine large volumes of data
  </li>
  <li>
    Give answers to real-world business questions
  </li>
  <li>
    Execute queries of various operational requirements and complexities (e.g., ad-hoc, reporting, iterative OLAP, data mining)
  </li>
  <li>
    Are characterized by high CPU and IO load
  </li>
  <li>
    Are periodically synchronized with source OLTP databases through database maintenance functions
  </li>
</ul>

To see additional benchmark details and results please <a href="http://www.tpc.org/tpcds/default.asp" target="_blank">Click Here</a>.

### TPC-E (Source : tpc.org)

TPC Benchmark E (TPC-E) is a new On-Line Transaction Processing (OLTP) workload developed by the TPC. The TPC-E benchmark uses a database to model a brokerage firm with customers who generate transactions related to trades, account inquiries, and market research. The brokerage firm in turn interacts with financial markets to execute orders on behalf of the customers and updates relevant account information.

The benchmark is scalable, meaning that the number of customers defined for the brokerage firm can be varied to represent the workloads of different-size businesses. The benchmark defines the required mix of transactions the benchmark must maintain. The TPC-E metric is given in transactions per second (tps). It specifically refers to the number of Trade-Result transactions the server can sustain over a period of time.

Although the underlying business model of TPC-E is a brokerage firm, the database schema, data population, transactions, and implementation rules have been designed to be broadly representative of modern OLTP systems.

To see additional benchmark details and results please <a href="http://www.tpc.org/tpce/results/tpce_results.asp" target="_blank">Click Here</a>.

### TPC-H (Source : tpc.org) 

The TPC Benchmark H (TPC-H) is a decision support benchmark. It consists of a suite of business oriented ad-hoc queries and concurrent data modifications. The queries and the data populating the database have been chosen to have broad industry-wide relevance. This benchmark illustrates decision support systems that examine large volumes of data, execute queries with a high degree of complexity, and give answers to critical business questions.

The performance metric reported by TPC-H is called the TPC-H Composite Query-per-Hour Performance Metric (QphH@Size), and reflects multiple aspects of the capability of the system to process queries. These aspects include the selected database size against which the queries are executed, the query processing power when queries are submitted by a single stream, and the query throughput when queries are submitted by multiple concurrent users. The TPC-H Price/Performance metric is expressed as $/QphH@Size.

To see additional benchmark details and results please <a href="http://www.tpc.org/tpch/results/tpch_results.asp?orderby=hardware" target="_blank">Click Here</a>.

### TPC-VMS (Source : tpc.org)

The TPC Virtual Measurement Single System Specification (TPC-VMS) leverages the TPC-C, TPC-E, TPC-H and TPC-DS Benchmarks by adding the methodology and requirements for running and reporting performance metrics for virtualized databases. The intent of TPC-VMS is to represent a Virtualization Environment where three database workloads are consolidated onto one server. Test sponsors choose one of the four benchmark workloads (TPC-C, TPC-E, TPC-H, or TPC-DS) and runs one instance of that benchmark workload in each of the 3 virtual machines (VMs) on the system under test. The 3 virtualized databases must have the same attributes, e.g. the same number of TPC-C warehouses, the same number of TPC-E Load Units, or the same TPC-DS or TPC-H scale factors.

The TPC-VMS Primary Performance Metric is the minimum value of the three TPC Benchmark Primary metrics for the TPC Benchmarks run in the Virtualization Environment.

To see additional benchmark details and results please <a href="http://www.tpc.org/tpcvms/default.asp" target="_blank">Click Here</a>.

### TPC-HS (Source : tpc.org) 

Big Data technologies like Hadoop have become an important part of the enterprise IT ecosystem. TPC Express Benchmark(tm)HS (TPCx-HS) was developed to provide an objective measure of hardware, operating system and commercial Apache Hadoop File System API compatible software distributions, and to provide the industry with verifiable performance, price-performance and availability metrics. The benchmark models a continuous system availability of 24 hours a day, 7 days a week.

The modeled application is simple and the results are highly relevant to hardware and software dealing with Big Data systems in general. The TPCx-HS stresses both hardware and software including Hadoop run-time, Hadoop Filesystem API compatible systems and MapReduce layers. This workload can be used to asses a broad range of system topologies and implementation of Hadoop clusters. The TPCx-HS can be used to asses a broad range of system topologies and implementation methodologies in a technically rigorous and directly comparable, in a vendor-neutral manner.

To see additional benchmark details and results please <a href="http://www.tpc.org/tpcx-hs/results/tpcxhs_results.asp" target="_blank">Click Here</a>.

### TPC-Energy (Source : tpc.org)

The TPC-Energy Specification contains the rules and methodology for measuring and reporting an energy metric in TPC Benchmarks. This includes the energy consumption of system components associated with typical business information technology environments, which are characterized by:

  * Energy consumption of servers
  * Energy consumption of disk systems
  * Energy consumption of other items that consume power and are required by the benchmark specification.

The measuring and publishing of the TPC-Energy Metrics in the TPC Benchmarks are optional and are not required to publish a TPC Result.

To see additional benchmark details and results please <a href="http://www.tpc.org/tpc_energy/default.asp" target="_blank">Click Here</a>.

