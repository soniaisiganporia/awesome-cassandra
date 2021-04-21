# Awesome Cassandra [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[<img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Cassandra_logo.svg" align="right" width="140">](http://cassandra.apache.org/)

Apache Cassandra is a free and open-source, distributed, wide column store, NoSQL database management system designed to handle large amounts of data across many commodity servers, providing high availability with no single point of failure.

This is a curated list of awesome [Apache Cassandra](http://cassandra.apache.org/) packages and resources. Maintained by Rahul Singh of [Anant](http://anant.us). Feel free contact me if you'd like to collaborate on this and other awesome lists. [Awesome Cassandra](https://github.com/Anant/awesome-cassandra) , [Awesome Solr](https://github.com/Anant/awesome-solr), [Awesome Lucene](https://github.com/Anant/awesome-lucene). This powers the *Resources* section of [Cassandra.Link](https://cassandra.link), a rich collection of blog feeds, and curated links as a searchable knowledge base.


## Contents

- [General](#general)
  - [Cassandra](#cassandra)
  - [Cassandra History](#cassandra-history)
  - [Cassandra Use Cases](#cassandra-use-cases)
  - [Cassandra Distributions](#cassandra-distributions)
  - [Using Cassandra](#using-cassandra)
  - [Cassandra from Relational](#cassandra-from-relational)
  - [Cassandra Data Modeling](#cassandra-data-modeling)
  - [Cassandra Architecture](#cassandra-architecture)
  - [Cassandra Monitoring](#cassandra-monitoring)
  - [Cassandra Maintenance](#cassandra-maintenance)
  - [Cassandra Performance Tuning](#cassandra-performance-tuning)
  - [Cassandra Security](#cassandra-security)
  - [Cassandra Deployment](#cassandra-deployment)
  - [Integrating with Cassandra](#integrating-with-cassandra)
- [Databases](#databases)
  - [Timeseries Databases](#timeseries-databases)
  - [Graph](#graph)
  - [Miscellaneous](#miscellaneous)
- [Packages](#packages)
  - [Libraries](#libraries)
  - [Tools](#tools)
  - [Open Source Applications](#open-source-applications)
  - [Logging /Metrics](#logging-metrics)
- [Resources](#resources)
  - [Documentation](#documentation)
  - [Books](#books)
  - [Courses](#courses)
  - [Communities](#communities)
  - [Blogs](#blogs)
  - [Videos](#videos)
  - [Slides](#slides)
  
## General

### Cassandra

- [Apache Cassandra](http://cassandra.apache.org/) - Manage massive amounts of data, fast, without losing sleep.

### Cassandra History

- [ZDNet: Apache Cassandra Turns 10](https://www.zdnet.com/article/apache-cassandra-turns-10/) - Highlights of the growth of Cassandra over it's first 10 years.

### Cassandra Use Cases

- [Datastax Academy: What is Cassandra?](https://www.datastax.com/cassandra) - Introduction to what Cassandra is, where it came from, and some of it's benefits.
- [Kaa application based on Raspberry Pi and DHT11 sensor](https://github.com/pyroalf/kaa-cassandra-sample) - Cassandra IoT usecase with Raspberry Pi and a DHT11 Sensor.
- [Simple Node.js Express 4 Cassandra Application](https://github.com/bradtraversy/mysubscribers) - MySubscribers is a very simple application (Start of an application) which allows you to create, read, update and delete users/subscribers. This application was only created to aid the YouTube course.
- [An Odyssey of Cassandra](http://hadoopmag.com/an-odyssey-of-cassandra/) - This is an old article republished but talks about transitioning from SQL to NoSQL with Cassandra.

### Cassandra Distributions

#### Cassandra Compliant Databases on JVM

<!-- double link - [Apache Cassandra](http://cassandra.apache.org/) - The original gangster for Cassandra is of course Apache Cassandra. Community supported. -->
- [Datastax Enterprise](https://www.datastax.com/) - Most widely used commercial distribution of Apache Cassandra, integrated with Apache Spark (for SparkSQL, analytics), Apache Solr (for secondary index), Apache TinkerPop based Graph stored in Cassandra, and OpsCenter.
- [DDAC/Luna](https://luna.datastax.com/) - Datastax Distribution of Apache Cassandra, a production ready distribution with a bulk loader supported by Datastax. DDAC is Deprecated now, but Datastax is still supporting Cassandra with it's new Luna Service.
<!-- - [Elassandra](http://www.elassandra.io/) - Elassandra = Elasticsearch as a Cassandra secondary index.  !Currently down as of 4/16/2021 12:50pm MST -->

#### Cassandra Compliant Databases on C++

- [ScyllaDB](https://github.com/scylladb/scylla) - NoSQL data store using the seastar framework, compatible with Apache Cassandra.
- [YugaByte Database](https://github.com/YugaByte/yugabyte-db) - YugaByteDB is a transactional, high-performance database for building distributed cloud services. It supports Cassandra-compatible and Redis-compatible APIs, with PostgreSQL in Beta.

#### Cassandra as a Service / Managed Cassandra Based on Open Source Cassandra

- [Datastax Astra](https://astra.datastax.com) - Datastax Astra Cassandra as a Service running on the Kubernetes operator Cassandra available on AWS and GCP.
- [Instaclustr Managed Apache Cassandra as a Service](https://www.instaclustr.com/solutions/managed-apache-cassandra/) - Instaclustr provides a fully managed and SOC 2 certified hosted & managed service for Apache Cassandra® on AWS, Azure, GCP and IBM Cloud.
- [Aiven for Apache Cassandra](https://aiven.io/cassandra/) - Aiven for Apache Cassandra is a managed and hosted distributed NoSQL database providing scalability, high availability, and excellent fault tolerance. Cassandra as a Service is available on Google Cloud Platform, Amazon Web Services, Microsoft Azure, DigitalOcean, and UpCloud.
- [Microsoft Azure Managed Instance for Apache Cassandra](https://docs.microsoft.com/en-us/azure/managed-instance-apache-cassandra/) - Azure Managed Instance for Apache Cassandra provides automated deployment and scaling operations for managed open-source Apache Cassandra datacenters. It accelerates hybrid scenarios and reduces ongoing maintenance.

#### Cassandra as a Service / Managed Cassandra Based on Proprietary Technology

- [Microsoft Azure Cosmos DB: Apache Cassandra API](https://docs.microsoft.com/en-us/azure/cosmos-db/cassandra-introduction) - Azure Cosmos DB provides the Cassandra API (preview) for applications that are written for Apache Cassandra that need premium capabilities.
- [Amazon Keyspaces for Apache Cassandra](https://aws.amazon.com/keyspaces) - Amazon Web Services (AWS) Amazon Keyspaces for Apache Cassandra provides a CQL compliant access to a "Serverless" auto-scaling datastore.

### Using Cassandra

<!-- - TODO:: cassandra installation tutorials in local, docker, cloud (do, aws, azure, gcp)) -->
<!-- - TODO:: compiling cassandra -->
<!-- - TODO:: running cassandra -->
<!-- - TODO:: using cql -->
<!-- - TODO:: using zeppelin with cassandra -->
<!-- - TODO:: getting data in / out of cassandra -->
<!-- - TODO:: using spark with cassandra -->
<!-- - [Install Cassandra and Spark](http://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html) - Quick user guide for integration with Cassandra and Spark. DOUBLE LINK ERROR IN AWESOME-LINT-->

- [Installing the Cassandra / Spark OSS Stack](https://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html) - Installation process and user guide for the Cassandra / Spark OSS Stack.
- [The Cassandra Query Language](http://cassandra.apache.org/doc/latest/cql/) - Documentation for CQL.
- [The LIMIT Clause in Apache Cassandra might not work as you think](http://thelastpickle.com/blog/2017/03/07/The-limit-clause-in-cassandra-might-not-work-as-you-think.html) - Blog post for the considerations on the efficiency of the LIMIT clause.
- [Building a Performant API using Go and Cassandra](https://getstream.io/blog/building-a-performant-api-using-go-and-cassandra/) - Tutorial documenting how to build a RESTful API using Go and Cassandra.
- [Cassandra Data Copy Tool](https://github.com/wildengineer/cassandra-data-copy-tool) - Java tool to copy data from one cassandra table to another.
- [Spring Data Cassandra Examples](https://github.com/jxblum/spring-data-cassandra-examples) - Examples for the Spring Data Cassandra Project.
- [Introduction to Spark & Cassandra](http://rustyrazorblade.com/post/2015/2015-01-02-intro-to-spark-and-cassandra/) - Blog post on setting up a really simple Spark job that does a data migration for Cassandra.
- [From Cassandra to S3, with Spark](https://objectpartners.com/2016/11/30/from-cassandra-to-s3-with-spark/) - Blog post showing how to connect Spark to Cassandra, analyze event data from Cassandra, and store the results of the analysis into S3, making it available for reporting or further analysis.
- [Import CSV files with spark](https://github.com/markthebault/importCSVSparkCassandra) - How to import a file from S3 into cassandra using Spark.
- [Top 5 reasons to use the Apache Cassandra Database](https://towardsdatascience.com/top-5-reasons-to-use-the-apache-cassandra-database-d541c6448557) - Few good reasons why you'd want to consider Apache Cassandra.
- [Cloud DevOps with Cassandra](http://cloudurable.com/blog/aws-ansible-packer-ssh-for-devops/index.html) - Using Packer, Ansible/SSH and AWS command line tools to create and DBA manage EC2 Cassandra instances in AWS.
- [How to install Cassandra 2 on CentOS 7 / RHEL 7](https://sharadchhetri.com/2015/04/25/how-to-install-cassandra-2-on-centos-7-rhel-7/) - Guide on how to install Cassandra on the popular linux distributions RedHat and CentOS.
- [Cassandra Use Cases: When to use and when not to use Cassandra](https://blog.pythian.com/cassandra-use-cases/) - Practical guide for when to use and when not to use Apache Cassandra.
- [Apache Cassandra Database (Guide)](https://www.instaclustr.com/education/apache-cassandra-database) - Great guide to learn about Apache Cassandra, from Instaclustr.

<!-- - TODO:: sql v. cql-->
<!-- - TODO:: query driven methodology -->
<!-- - TODO:: schema designs / examples-->
<!-- - TODO:: data modeling problems -->

### Cassandra from Relational

- [RDBMS to NoSQL](http://www.datastax.com/relational-database-to-nosql) - Your roadmap to understanding whether NoSQL is right for you.
- [Cassandra Schemas for Beginners (like me)](https://medium.com/@jochasinga/cassandra-schemas-for-beginners-like-me-9714cee9236a) - Great article for new developers to Cassandra.
- [Cassandra Query Language: CQL vs SQL](https://medium.com/@alexbmeng/cassandra-query-language-cql-vs-sql-7f6ed7706b4c) - Blog post documenting similarities and differences between CQL and SQL.
<!-- - [MySQL to C*](http://planetcassandra.org/mysql-to-cassandra-migration/) - MySQL to Cassandra migration guide.  !This is just redirecting to https://www.datastax.com/dev -->
<!-- - [Cassandra and Relational database schema comparison – Query vs relationship modeling](https://blog.rdx.com/cassandra-and-relational-database-schema-comparison-query-vs-relationship-modeling/) - Lacking security certificate as of 4/12/2021 @ 8:50 am MST -->
<!-- - [Real-Time Replication from MySQL to Cassandra](https://mcbguru.blog/2014/02/27/real-time-replication-from-mysql-to-cassandra/) - Website is down as of 4/12/2021 @ 8:47 am MST -->

### Cassandra Data Modeling

<!-- awesome-lint Throwing Double Link Error - [Cassandra Query Language : CQL vs. SQL](https://medium.com/@alexbmeng/cassandra-query-language-cql-vs-sql-7f6ed7706b4c) - Blog post documenting similarities and differences between CQL and SQL. -->
- [Basic Rules Of Cassandra Data Modeling](http://www.datastax.com/dev/blog/basic-rules-of-cassandra-data-modeling) - Picking the right data model is the hardest part of using Cassandra. If you have a relational background, CQL will look familiar, but the way you use it can be very different.
- [CQL: This is not the SQL you are Looking For](https://www.slideshare.net/aploetz/cql-this-is-not-the-sql-you-are-loooking-for) - This presentation will explore and explain the differences between the CQL and SQL languages.
- [A Deep Look at the CQL Where Clause](https://www.datastax.com/dev/blog/a-deep-look-to-the-cql-where-clause) - Blog post to describe what is supported by the CQL WHERE clause and the reasons why it differs from normal SQL.
- [killrvideo-sample-schema](https://github.com/pmcfadin/killrvideo-sample-schema) - Sample Cassandra CQL Schema for a YouTube clone.
- [Spring Data Cassandra Examples](https://github.com/jxblum/spring-data-cassandra-examples/blob/master/src/main/resources/cassandra-example-schema.cql) - This Maven project contains examples showcasing the features and functionality of the Spring Data Cassandra project.
- [Common Problems in Cassandra Data Models](https://blog.anant.us/common-problems-cassandra-data-models/) - Presentation and Article on wide partions, tombstones, and data skew.
- [Casandra Time Series Data Modeling for Massive Scale](http://thelastpickle.com/blog/2017/08/02/time-series-data-modeling-massive-scale.html) - Blog post discussing a common Cassandra data modeling technique called bucketing.
- [Cassandra Data Modeling Notes](https://miguelperez.xyz/blog/2017/2/13/cassandra-data-modeling-notes) - Simple notes on how to estimate the size of your cluster.
- [Scalar DB](https://github.com/scalar-labs/scalardb) - Transaction library for Cassandra that makes non-ACID distributed databases/storages ACID-compliant.
- [Cassandra Data Modeling Best Practices Guide](https://www.instaclustr.com/cassandra-data-modeling/) - Explains five Cassandra data modeling best practices.

<!-- - TODO: - Data Centers and Racks -->
<!-- - TODO: - Gossip and Failure Detection -->
<!-- - TODO: - Snitches -->
<!-- - TODO: - Rings and Tokens -->
<!-- - TODO: - Virtual Nodes -->
<!-- - TODO: - Partitioners -->
<!-- - TODO: - Replication Strategies -->
<!-- - TODO: - Consistency Levels -->
<!-- - TODO: - Queries and Coordinator Nodes -->
<!-- - TODO: - Memtables, SSTables, and Commit Logs -->
<!-- - TODO: - Caching -->
<!-- - TODO: - Hinted Handoff -->
<!-- - TODO: - Lightweight Transactions and Paxos -->
<!-- - TODO: - Tombstones -->
<!-- - TODO: - Bloom Filters -->
<!-- - TODO: - Compaction -->
<!-- - TODO: - Anti-Entropy, Repair, and Merkle Trees -->
<!-- - TODO: - Staged Event-Driven Architecture (SEDA) -->
<!-- - TODO: - Managers and Services -->
<!-- - TODO: - System Keyspaces -->

### Cassandra Architecture

- [The Gossip Protocol - Inside Apache Cassandra.](https://www.linkedin.com/pulse/gossip-protocol-inside-apache-cassandra-soham-saha) - Good visual explanation of how Cassandra keeps consistent.
- [Introduction To The Apache Cassandra 3.x Storage Engine](http://thelastpickle.com/blog/2016/03/04/introductiont-to-the-apache-cassandra-3-storage-engine.html) - The 3.x storage engine makes it easier for Cassandra to get bytes off disk.
- [Dropping columns in Apache Cassandra 3.0](http://thelastpickle.com/blog/2016/02/18/dropping-columns.html) - Blog post describing the steps Cassandra takes when a column is dropped.
- [Hinted Handoff and GC Grace Demystified](http://thelastpickle.com/blog/2018/03/21/hinted-handoff-gc-grace-demystified.html) - Tuning the balance between GC Grace and Hinted Handoff.
- [Deletes and Tombstones](http://thelastpickle.com/blog/2011/05/15/Deletes-and-Tombstones.html) - Explains how deletes create tombstones in Cassandra and what they are.
- [About Deletes and Tombstones in Cassandra](http://thelastpickle.com/blog/2016/07/27/about-deletes-and-tombstones.html) - Deleting distributed and replicated data from a system such as Apache Cassandra is far trickier than in a relational database.
- [Null bindings on prepared statements and undesired tombstone creation](http://thelastpickle.com/blog/2016/09/15/Null-bindings-on-prepared-statements-and-undesired-tombstone-creation.html) - Good follow up to the last article on Tombstones.
- [Undetectable tombstones in Apache Cassandra](http://thelastpickle.com/blog/2018/07/05/undetectable-tombstones-in-apache-cassandra.html) - Indepth analysis of cell and range tombstones.
- [Common Problems with Cassandra Tombstones](https://opencredo.com/cassandra-tombstones-common-issues/) - Large number of tombstones causes Latency and heap pressure.
- [Curious Case of Tombstones](https://medium.com/cassandra-tombstones-clearing-use-case/the-curios-case-of-tombstones-d897f681a378) - How someone dealt with tombstone issues and reclaimed space in their cluster.
- [Understanding the Nuance of Compaction in Apache Cassandra](http://thelastpickle.com/blog/2017/03/16/compaction-nuance.html) - Overview of how Cassandra manages data on disk.
- [Guide to Cassandra Thread Pools](https://blog.pythian.com/guide-to-cassandra-thread-pools/) - This guide provides a description of the different thread pools and how to monitor them. Includes what to alert on, common issues and solutions. Old but very useful reference.
- [Cassandra Architecture and Operations](https://miguelperez.xyz/blog/2017/2/13/cassandra-architecture-and-operation) - High level overview in one page of how Cassandra works.
- [Improving Apache Cassandra's Front Door and Backpressure](https://dzone.com/articles/improving-apache-cassandras-front-door-and-backpre) - Explore how an incoming request was processed by Cassandra before, see what they changed, and look at new relevant configuration knobs available.
- [Cassandra Architecture](https://www.instaclustr.com/cassandra-architecture/) - High level overview of Apache Cassandra from Instaclustr.
- [The 10 Things I hate about Apache Cassandra](https://blog.pythian.com/the-things-i-hate-about-apache-cassandra/) - Do you really want to use Apache Cassandra? Learn why not to use it.

### Cassandra Monitoring

- [Resources for Monitoring Datastax, Cassandra, Spark, & Solr Performance](https://blog.anant.us/resources-for-monitoring-datastax-cassandra-spark-solr-performance/) - Blogpost detailing different types of monitoring tools and their purpose.
- [How to Monitor Cassandra](https://www.datadoghq.com/blog/how-to-monitor-cassandra-performance-metrics/) - Guide to help you monitor Cassandra performance and work metrics regardles of which monitoring tool you choose to use.
- [Cassandra metrics and their use in Grafana](https://medium.com/@mlowicki/cassandra-metrics-and-their-use-in-grafana-1f0dc33f9cca) - Case study of using Cassandra metrics in Grafana.
- [Monitoring Cassandra with Prometheus](https://www.robustperception.io/monitoring-cassandra-with-prometheus) - Quick setup guide to using Cassandra with Prometheus.
- [Monitoring Cassandra With Grafana And Influx DB](https://blog.pythian.com/monitoring-cassandra-grafana-influx-db/) - Blogpost explaining how to set up Cassandra monitoring with influxDB and Grafana.
- [Cassandra Monitoring - Introduction (1/2)](https://softwaremill.com/cassandra-monitoring-part-1/) - Blogpost detailing how Cassandra metrics can be gathered.
- [Cassandra Monitoring - Graphite/InfluxDB & Grafana on Docker (2/2)](https://softwaremill.com/cassandra-monitoring-part-2/) - Continuation of the previous entry exploring the topic of Cassandra metric reporters mentioned in Part I. The goal is to configure a reporter that sends metrics to an external time series database.
- [Monitoring Cassandra using Intel Snap and Grafana](http://thelastpickle.com/blog/2017/04/13/monitoring-cassandra-using-intel-snap.html) - This blog post describes how to monitor Apache Cassandra using the Intel Snap open source telemetry framework.
- [Cassandra Monitoring Best Practice Guide](https://www.instaclustr.com/cassandra-monitoring-best-practice-guide/) - This blog post aims to touch all important aspects of Cassandra monitoring.

<!-- - TODO:: Health Check -->
<!-- - TODO:: Basic Maintenance -->
<!-- - TODO:: Adding Nodes -->
<!-- - TODO:: Handling Node Failure -->
<!-- - TODO:: Upgrading Cassandra -->
<!-- - TODO:: Backup and Recovery -->
<!-- - TODO:: SSTable Utilities -->
<!-- - TODO:: Maintenance Tools  -->
<!--  - OpsCenter  -->
<!--  - Reaper  -->
<!--  - TableAnalyzer  -->

### Cassandra Maintenance

- [Running commands cluster-wide without any management tool](http://thelastpickle.com/blog/2016/03/21/running-commands-cluster-wide.html) - Some tips and tricks to do basic Cluster operations without tools like Chef, Ansible, or Salt.
- [Limiting Nodetool Parallel Threads](http://thelastpickle.com/blog/2017/08/14/limiting-nodetool-parallel-threads.html) - Little known tool to do nodetool operations with less resources.
- [Bootstrapping Cassandra Nodes](http://thelastpickle.com/blog/2017/05/23/auto-bootstrapping-part1.html) - Indepth article on how to add nodes to a running Cassandra cluster.
- [Node Replacement without Bootstrapping](http://thelastpickle.com/blog/2018/02/21/replace-node-without-bootstrapping.html) - How to avoid the long bootstrapping process.
- [Cassandra Backup and Restore - Backup in AWS using EBS Volumes](http://thelastpickle.com/blog/2018/04/03/cassandra-backup-and-restore-aws-ebs.html) - Indepth article about Backup and recovery in AWS.
- [Backup Strategies for Cassandra](https://blog.pythian.com/backup-strategies-cassandra/) - Good comparison of different backup and restoration strategies for Cassandra.
- [Cassandra backup util](https://github.com/instaclustr/cassandra-backup) - Instaclustr's cassandra backup tool.
- [Cassy](https://github.com/scalar-labs/cassy) - Simple and integrated backup tool for Apache Cassandra.
- [Intro to CStar](https://thelastpickle.com/blog/2018/10/01/introduction-to-cstar.html) - Tutorial on how to use CStar.
- [Medusa](https://github.com/thelastpickle/cassandra-medusa) - Apache Cassandra backup system.
<!-- double-link - [cassandra-sstable-tools](https://github.com/instaclustr/cassandra-sstable-tools) - Tools for working with sstables. -->
<!-- double-link - [sstable tools](https://github.com/tolbertam/sstable-tools) - A toolkit for parsing, creating and doing other fun stuff with Cassandra 3.x SSTables. -->

<!-- - TODO:: Managing Performance -->
<!-- - TODO:: Caching -->
<!-- - TODO:: Memtables -->
<!-- - TODO:: Commit Logs -->
<!-- - TODO:: SSTables -->
<!-- - TODO:: Hinted Handoff -->
<!-- - TODO:: Compaction -->
<!-- - TODO:: Concurrency and Threading -->
<!-- - TODO:: Networking and Timeouts -->
<!-- - TODO:: JVM Settings -->
<!-- - TODO:: Using cassandra-stress -->
<!-- - TODO:: Using Gatling -->

### Cassandra Performance Tuning

- [Jon Haddad: Cassandra Summit Recap - Diagnosing Problems in Production](http://rustyrazorblade.com/2014/09/cassandra-summit-recap-diagnosing-problems-in-production/)
- [Ryan Svihla's Cassandra 2.0 checklist](https://medium.com/@foundev/my-cassandra-diagnostics-checklist-brain-dump-599a2b95b118) - Checklist for determining the efficiency of your Cassandra database.
- [Amy's Cassandra 2.1 tuning guide](https://tobert.github.io/pages/als-cassandra-21-tuning-guide.html) - Guide to tracking down performance issues in production level Cassandra clusters.
- [Secret HotSpot option improving GC pauses on large heaps](http://blog.ragozin.info/2012/03/secret-hotspot-option-improving-gc.html)
- [DSE 5.1: Tuning Java Resource](https://docs.datastax.com/en/dse/5.1/dse-admin/datastax_enterprise/operations/opsTuneJVM.html) - Documentation for tuning JVM.
- [Analyzing Cassandra Performance with Flame Graphs](http://thelastpickle.com/blog/2018/01/16/cassandra-flame-graphs.html) - Visually examining Cassandra performance visually using Flamegraphs.
- [Garbage Collection Tuning for Cassandra](http://thelastpickle.com/blog/2018/04/11/gc-tuning.html) - Optimizing garbage collection for better performance.
- [Cassandra Node Diagnostics Tools](https://github.com/smartcat-labs/cassandra-diagnostics) - Monitoring and audit power kit for Apache Cassandra.
- [TWCS part 1 - how does it work and when should you use it?](http://thelastpickle.com/blog/2016/12/08/TWCS-part1.html) - Best suited for time series data that expires, Time Window Compaction Strategy comes with some caveats.
- [Performing User Defined Compactions in Apache Cassandra](http://thelastpickle.com/blog/2016/10/18/user-defined-compaction.html) - Documenting a process by which we tell Cassandra to create a compaction task for one or more tables explicitly.
- [Graphing cassandra-stress](http://thelastpickle.com/blog/2015/10/23/cassandra-stress-and-graphs.html) - Benchmarking schemas and configuration changes using the cassandra-stress tool, before pushing such changes out to production is one of the things every Cassandra developer should know and regularly practice.
- [Modeling real life workloads with cassandra-stress is hard](http://thelastpickle.com/blog/2017/02/08/Modeling-real-life-workloads-with-cassandra-stress.html) - Blogpost detailing caveats with cassandra-stress when modeling real workloads.
- [Gatling DSE Stress](https://github.com/datastax/gatling-dse-stress)
- [Gatling DSE Plugin for Gatling Load injector](https://github.com/datastax/gatling-dse-plugin) - Plugin for the Gatling load injector. It adds CQL support in Gatling for Datastax Enterprise. It allows for benchmarking Datastax Enterprise features, including DSE Graph Fluent API.
- [Gatling DSE Stress Simulation Catalog](https://github.com/datastax/gatling-dse-simcatalog) - The goal of the repo is to provide a sample of the Gatling DSE Stress Framework's usage. Feel free to submit a pull request with example simulations.
<!-- !Now just redirects to https://www.datastax.com/dev - [A Deeper Dive - Diagnosing DSE Performance Issues with Ttop and Multidump](https://academy.datastax.com/support-blog/deeper-dive-diagnosing-dse-performance-issues-ttop-and-multidump) - A good review of how to look deeper into Cassandra threads. -->

<!-- - TODO:: Authentication and Authorization -->
<!-- - TODO:: Encryption -->
<!-- - TODO:: JMX Security -->
<!-- - TODO:: Disk -->
<!-- - TODO:: System -->
<!-- - TODO:: Network -->

### Cassandra Security

- [Securing Apache Cassandra with Application Level Encryption](https://www.instaclustr.com/securing-apache-cassandra-with-application-level-encryption/) - Discusses how to do application level data encryption to properly manage secure information in Cassandra.
- [Hardening Cassandra Step by Step: Part 1](http://thelastpickle.com/blog/2015/09/30/hardening-cassandra-step-by-step-part-1-server-to-server.html) - Inter-Node Encryption (And a Gentle Intro to Certificates).
- [LDAP Authenticator for Apache Cassandra](https://github.com/instaclustr/cassandra-ldap) - Pluggable authentication implementation for Apache Cassandra, providing a way to authenticate and create users based on a configured LDAP server.
- [Encrypting EC2 ephemeral volumes with LUKS and AWS KMS](https://www.whaletech.co/2016/04/07/encryption-ephemeral-volumes-with-kms.html) - The example used here is Cassandra data stored on ephemeral disks.

<!-- - TODO:: Container Deployment -->
<!-- - TODO:: Container Orchestration -->
<!-- - TODO:: Cloud Deployment -->
<!-- - TODO:: Cloud Automations -->

### Cassandra Deployment

- [An Introduction to Cassandra Multi-Data Centers: Part 1](https://www.instaclustr.com/around-the-world-in-approximately-8-data-centres-globally-distributed-storage-streaming-and-search-part-1/) - Learn about how to plan and implement Multi-Data Centers: Part 1.
- [An Introduction to Cassandra Multi-Data Centers: Part 2](https://www.instaclustr.com/around-the-world-globally-distributed-storage-streaming-and-search-an-introduction-to-cassandra-multi-data-centers-part-2/) - Learn about how to plan and implement Multi-Data Centers: Part 2.
- [How To Setup A Highly Available Multi-AZ Cassandra Cluster On AWS EC2](http://highscalability.com/blog/2016/8/1/how-to-setup-a-highly-available-multi-az-cassandra-cluster-o.html)
- [tlp-cluster, a tool for launching Cassandra clusters in AWS](https://github.com/thelastpickle/tlp-cluster) - A provisioning tool for Apache Cassandra designed for developers looking to both benchmark and test the correctness of Apache Cassandra. It assists with builds and starting instances on AWS.
- [Setting Up Cassandra Cluster Through Ansible](https://blog.knoldus.com/setting-up-cassandra-cluster-through-ansible/) - A guide detailing how to set up a Cassandra cluster with automation using Ansible.
- [Running Cassandra on DC/OS (Mesos)](http://thelastpickle.com/blog/2016/05/07/dcos.html) -  This blog will show how to setup DC/OS in the Amazon cloud, how to install Apache Cassandra on a DC/OS cluster, and finally new ways to interact with and Apache Cassandra after it is installed.
- [Benchmarking Cassandra with Local Storage on Azure](https://www.instaclustr.com/benchmarking-cassandra-with-local-storage-on-azure/) - Learn about comparing Cassandra on Azure VMs w/ Local vs. Remote storage.  
<!-- !LoyaltyOne's repos are now all private 404 - [CloudFormation Cassandra AWS](https://github.com/LoyaltyOne/cassandra-aws) - A cassandra cluster for development using Cloud Formation. -->

#### Cassandra Deployment on Docker / Containerized Cassandra

- [Docker Meet Cassandra. Cassandra Meet Docker](http://thelastpickle.com/blog/2018/01/23/docker-meet-cassandra.html) - Article reviewing how to setup a complete Cassandra application with monitoring on Docker.
- [Example code from the Docker Meet Cassandra Article](https://github.com/thelastpickle/docker-cassandra-bootstrap)
- [Docker-Cassandra](https://github.com/nicolasff/docker-cassandra) - A set of scripts and config files to run a Cassandra cluster from Docker.
- [Cassandra & Zeppelin Notebook on Docker](https://github.com/academyofdata/cassandra-zeppelin) - Docker-Compose script for Cassandra + Zeppelin setup.
- [Packer: Cassandra Image](https://github.com/cloudurable/cassandra-image) - Cassandra Image using Packer for Docker and EC2 AMI. Covers managing EC2 Cassandra clusters with Ansible.
- [Cassandra Docker](https://github.com/instaclustr/cassandra-docker) - This is the Instaclustr public docker image for Apache Cassandra. It contains docker images for Cassandra 3.0 and 3.11.1.
- [Cassandra / Elassandra Docker](https://github.com/zegelin/cassandra-docker) - Apache Cassandra and Elassandra docker images.Cass Operator is maintained by a team at DataStax and it is part of what powers DataStax Astra.

#### Cassandra Deployment on Kubernetes / Kubernetized Cassandra

- [K8ssandra.io - Kubernetes + Cassandra](https://k8ssandra.io/) - K8ssandra provides a production-ready platform for running Apache Cassandra on Kubernetes. This includes automation for operational tasks such as repairs, backups, and monitoring.
- [Datastax - Cassandra Kubernetes Operator](https://github.com/datastax/cass-operator) - Datastax's Cassandra Kubernetes Operator which supports Datastax as well as open source Apache Cassandra containers on Kubernetes.
- [Instaclustr - Kubernetes Operator for Cassandra](https://github.com/instaclustr/cassandra-operator) - The Cassandra operator manages Cassandra clusters deployed to Kubernetes and automates tasks related to operating an Cassandra cluster.
- [Sky UK - Cassandra Kubernetes Operator](https://github.com/sky-uk/cassandra-operator) - Kubernetes operator that manages Cassandra clusters inside Kubernetes. Well designed and organized.
- [CassKop - Cassandra operator for Kubernetes](https://github.com/Orange-OpenSource/cassandra-k8s-operator) - This Kubernetes operator automates the Cassandra operations such as deploying a new rack aware cluster, adding/removing nodes, configuring the C and JVM parameters, upgrading JVM and C versions. Written in Go.
- [Strapdata - Elassandra Operator for Kubernetes](https://github.com/strapdata/elassandra-operator) - The Elassandra Kubernetes Operator automates the deployment and management of Elassandra clusters deployed in multiple Kubernetes clusters.
- [Rook.io - Cassandra on Kubernetes](https://rook.io/docs/rook/v1.4/cassandra.html) - Rook is an open source cloud-native storage orchestrator, providing the platform, framework, and support for a diverse set of storage solutions to natively integrate with cloud-native environments. They have a special operator for Apache Cassandra amongst other providers.
- [Kudo Cassandar Operator](https://github.com/mesosphere/kudo-cassandra-operator) - The KUDO Cassandra Operator makes it easy to deploy and manage Apache Cassandra on Kubernetes.

### Integrating with Cassandra

- [Building a Streaming Data Hub with Elasticsearch, Kafka and Cassandra](http://thenewstack.io/building-streaming-data-hub-elasticsearch-kafka-cassandra/) - Blogpost detailing how a streaming analytics system on top of open source, big data components can be done.
- [Docker container for Kafka - Spark streaming - Cassandra](https://github.com/Yannael/kafka-sparkstreaming-cassandra) - Dockerfile that sets up a complete streaming environment for experimenting with Kafka, Spark streaming (PySpark), and Cassandra.
- [sample KafkaSparkCassandra](https://github.com/instaclustr/sample-KafkaSparkCassandra) - Introductory sample scala app using Apache Spark Streaming to accept data from Kafka and write a summary to Cassandra.
- [sample Spark Cassandra with SSL](https://github.com/instaclustr/sample-SparkCassandrawithSSL) - Simple sample job illustrating the use of Spark to execute Apache Spark analytics with Cassandra with SSL connection.

<!-- - TODO:: ESB -->
<!-- - TODO:: Streaming -->
<!-- - TODO:: ETL -->
<!-- - TODO:: CDC -->

#### Spark

- [DataStax Spark Cassandra Connector](https://github.com/datastax/spark-cassandra-connector) - This library lets you expose Cassandra tables as Spark RDDs, write Spark RDDs to Cassandra tables, and execute arbitrary CQL queries in your Spark applications.
- [Stratio Deep (deprecated)](https://github.com/Stratio/stratio-deep) - Deep is a thin integration layer between Apache Spark and several NoSQL datastores. We actually support Apache Cassandra and MongoDB, but in the near future we will add support for sever other datastores.
- [sample Spark Job Server Cassandra](https://github.com/instaclustr/sample-SparkJobserverCassandra) - Simple sample job illustrating the use of Spark Jobserver to execute Apache Spark analytics with Cassandra.
- [fluxcapacitor/pipeline](https://github.com/fluxcapacitor/pipeline) - End-to-End, Real-time, Advanced Analytics Big Data Reference Pipeline using Spark, Spark SQL, Spark ML, GraphX, Spark Streaming, Kafka, NiFi, Cassandra, ElasticSearch, Redis, Tachyon, HDFS, Zeppelin, iPython/Jupyter Notebook, Tableau, Twitter Algebird.
- [Spark + Cassandra Best Practices](https://blog.pythian.com/spark-cassandra-best-practices/) - Outlines general use cases and best practices of Spark & Cassandra together.

#### Search / Secondary Indexes

- [Tuning DSE Search](http://www.datastax.com/dev/blog/tuning-dse-search) - Tuning DSE Search – Indexing latency and query latency.
- [Cassandra Lucene Index](https://github.com/Stratio/cassandra-lucene-index) - Lucene based secondary indexes for Cassandra.
- OLD - [Solandra](https://github.com/tjake/Solandra) - Solandra is a real-time distributed search engine built on Apache Solr and Apache Cassandra.
- [cassandra-trigger](https://github.com/gradeup/cassandra-trigger) - Cassandra trigger to push realtime updates to elasticsearch.
<!-- double-link - [Elassandra](http://www.elassandra.io/) - Elassandra = Elasticsearch as a Cassandra secondary index. -->

## Databases

### Timeseries Databases

#### Monitoring / Metrics

- [cortexproject/cortex](https://github.com/cortexproject/cortex) - Horizontally scalable, highly available, multi-tenant, long term Prometheus storage.
- [filodb/FiloDB](https://github.com/filodb/FiloDB) - Distributed Prometheus time-series database compatible with Prometheus queries.
- [cybem/cyanite-iow](https://github.com/cybem/cyanite-iow) - Cassandra backed Carbon daemon and metric web service. IPONWEB repository, compatible with Carbon.

#### Custom Time Series

- [Spotify/Heroic](https://github.com/spotify/heroic) - The, now deprecated, Heroic Time Series Database built by Spotify which works on Cassandra and Elasticsearch. The authors mention it will no longer be updated, but should work bug-free.
- [Heroic Documentation](https://spotify.github.io/heroic/docs/overview) - The Heroic Time Series Database documentation.
- [kairosdb/kairosdb](https://github.com/kairosdb/kairosdb) - Fast scalable time series database. 
- [Cassandra Schema — KairosDB 1.0.1 documentation](https://kairosdb.github.io/docs/build/html/CassandraSchema.html) - KairosDB documentation.
- [Newts](https://opennms.github.io/newts/) - Time-series data store based on Apache Cassandra.
- [OpenNMS/newts](https://github.com/OpenNMS/newts) - New-fangled Timeseries Data Store that powers OpenNMS.
- [Hawkular.org](https://www.hawkular.org/) - A time series / distributed tracing database powered by Cassandra by Redhat.
- [Hawkular GitHub](https://github.com/hawkular) - Hawkular's GitHub resources.
- [OpenTSDB/opentsdb](https://github.com/OpenTSDB/opentsdb) - GitHub resources for OpenTSDB. A Distributed, Scalable Monitoring System built on a Time Series Database.
<!-- !Unsecure website warning - [OpenTSDB](https://opentsdb.net/) - A Distributed, Scalable Monitoring System built on a Time Series Database. -->
<!-- !Seems to be unmaintained now, build failing tags - [rackerlabs/blueflood](https://github.com/rackerlabs/blueflood) - GitHub resources for blueflood. -->
<!-- !Unsecure website warning - [blueflood.io](https://blueflood.io/) - A distributed system designed to ingest and process time series data. -->

### Graph

- [DSE Graph | Datastax](https://www.datastax.com/products/datastax-graph) - Successor to TitanDB , Commercial Tinkerpop / Gremlin compatible large scale Graph Database on DSE.
- [Thinkaurelius/Titan](https://github.com/thinkaurelius/titan) - Distributed Graph Database, predecessor to DSE Graph, JanusGraph, and now HugeGraph.
- [Introduction to TitanDB](https://www.slideshare.net/knoldus/introduction-to-titandb) - Introductory slides about TitanDB.
- [JanusGraph/janusgraph](https://github.com/JanusGraph/janusgraph) - JanusGraph: an open-source, distributed graph database, successor to TitanDB.
- [Large Scale Graph Analytics with JanusGraph](https://www.slideshare.net/Hadoop_Summit/large-scale-graph-analytics-with-janusgraph-77153443) - Slides detailing deployment options and technical aspects of JanusGraph.
- [Hugegraph/Hugegraph](https://github.com/hugegraph/hugegraph) - HugeGraph Database core component, including graph engine, API, and built-in backends.
- [Architecture Overview · GitBook](https://hugegraph.github.io/hugegraph-doc/guides/architectural.html) - Documentation for HugeGraph.

### Miscellaneous

- [Stargate](https://github.com/stargate/stargate) - Stargate is an open-source data gateway that provides REST, GraphQL and schemaless JSON interfaces to Cassandra.
- [Meet Stargate, DataStax's GraphQL for databases. First stop - Cassandra](https://www.zdnet.com/article/meet-stargate-datastaxs-graphql-for-databases-first-stop-cassandra/) - Introduction and high-level overview of Stargate.
- [Apache/Usergrid](https://github.com/apache/usergrid) - Open source Backend as a Service (BaaS) on Apache Cassandra, Elasticsearch with client SDKs for iOS/Android/.NET/Java.
- [Building Your Own BaaS With Apache Usergrid &amp; Docker: Lessons Learned At Scale](http://events17.linuxfoundation.org/sites/events/files/slides/Building%20Your%20Own%20BaaS%20With%20Apache%20Usergrid%20%26%20Docker.pdf) - Introductory presentation to Apache UserGrid.
- [Scalar-labs/Scalardl](https://github.com/scalar-labs/scalardl) - Tamper-evident and scalable distributed ledger platform.
- [Wikimedia/Restbase](https://github.com/wikimedia/restbase) -  Distributed storage with REST API &amp; dispatcher for backend services.
- [Wikimedia/restbase-mod-table-spec](https://github.com/wikimedia/restbase-mod-table-spec) - Shared spec and tests for RESTBase table storage.
<!-- double-link - [scalar-labs/scalardb](https://github.com/scalar-labs/scalardb) - Library that makes non-ACID distributed databases/storages ACID-compliant. -->

## Packages

### Libraries

- [express-cassandra](https://github.com/masumsoft/express-cassandra) - Cassandra ORM/ODM/OGM for Node.js with optional support for Elassandra & JanusGraph.
- [DataStax Java Driver](https://github.com/datastax/java-driver) - A Java client driver for Apache Cassandra.
- [DataStax C++ Driver](https://github.com/datastax/cpp-driver) - A modern, feature-rich, and highly tunable C/C++ client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's native protocol and Cassandra Query Language v3.
- [DataStax Python Driver](https://github.com/datastax/python-driver) - A modern, feature-rich and highly-tunable Python client library for Apache Cassandra (2.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax Ruby Driver](https://github.com/datastax/ruby-driver) - A Ruby client driver for Apache Cassandra. This driver works exclusively with the Cassandra Query Language version 3 (CQL3) and Cassandra's native protocol.
- [DataStax Node.js Driver](https://github.com/datastax/nodejs-driver) - A modern, feature-rich and highly tunable Node.js client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax C# Driver](https://github.com/datastax/csharp-driver) - A modern, feature-rich and highly tunable C# client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax PHP Driver](https://github.com/datastax/php-driver) - DataStax PHP Driver for Apache Cassandra.
- [Achilles](http://doanduyhai.github.io/Achilles/) - Achilles is an open source Persistence Manager for Apache Cassandra,with the features like Advanced bean mapping (compound primary key, composite partition key, timeUUID, ect),Native collections and map support,and so.
- [phpcassa](https://github.com/thobbs/phpcassa) - PHP client library for Apache Cassandra.
- [Caffinitas](https://bitbucket.org/snazy/caffinitas/src/develop/) - Caffinitas is an advanced object mapper for Apache Cassandra which has been especially designed to work with Datastax Java Driver 2.1+ against Apache Cassandra 2.1, 2.0 or 1.2.
- [Spring Data for Apache Cassandra](http://projects.spring.io/spring-data-cassandra/) -  Spring Data for Apache Cassandra offers a familiar interface to those who have used other Spring Data modules in the past.
- [gocql](https://github.com/gocql/gocql) - Package gocql implements a fast and robust Cassandra client for the Go programming language.
- [Netflix Astyanax](https://github.com/Netflix/astyanax) - This is an old library. Astyanax was a high level Java client for Apache Cassandra, based on Thrift protocol. Not maintained any more.

### Tools

- [Hackolade](https://hackolade.com) - Visual data modeling tool for NoSQL databases and stuctures like Apache Cassandra, ElasticSearch, Graph DBs, JSON, APIs.  
- [JetBrains Datagrip DB IDE](https://www.jetbrains.com/datagrip/) - The Cross-Platform IDE for Databases & SQL by JetBrains, with support for Cassandra.
- [Datastax - Management API for Apache Cassandra](https://github.com/datastax/management-api-for-apache-cassandra) - The Management API is a sidecar service layer that attempts to build a well supported set of operational actions on Cassandra® nodes that can be administered centrally.
- [DataStax OpsCenter](http://www.datastax.com/what-we-offer/products-services/datastax-opscenter) - Simplified management for DataStax Enterprise and Cassandra database clusters.
- [CassandraCAS](https://github.com/Datomic/CassandraCAS) - Compare-and-swap tool for Cassandra created by Datomic.
- [Peloton](https://github.com/uber/peloton) - Unified resource scheduler created by Uber. This tool can handle many nodes and clusters through resource management and scalability.
- [Ansible-Galaxy: Cassandra GitHub](https://github.com/ansible-collections/community.cassandra) - This collection called cassandra aims at providing all Ansible modules allowed to interact with Apache Cassandra. 
- [Ansible-Galaxy: Cassandra](https://galaxy.ansible.com/community/cassandra) - Documentation for Ansible-Galaxy: Cassandra.
- [Ansible-dse](https://github.com/rackerlabs/ansible-dse) - Set of Ansible playbooks that will build a Datastax Enterprise cluster.
- [dseansible](https://github.com/yabinmeng/dseansible) - DSE Installation and Upgrade Ansible Playbooks/Roles for Ubuntu Linux.
- [DbSchema - Cassandra Designer](https://dbschema.com/database-designer/Cassandra.html) - DbSchema: Cassandra Diagram Designer & GUI Admin Tool which can do Cassandra amongst other databases.
- [DBeaver - Free Universal Database Tool](https://dbeaver.io/) - Third party tool for dealing with all sorts of databases including Cassandra.
- [RazorSQL - Multi DB Manager Tool](https://razorsql.com/) - Multi-db tool for Linux, Mac, and Windows that works with Apache Cassandra.
- [KDM - The Kashlev Data Modeler](http://kdm-portal.weebly.com/) - Automated big data modeling tool for Apache Cassandra.
- [Cassandra Reaper](http://cassandra-reaper.io/) - Automated repairs for Apache Cassandra. Supports all versions.
- [cstar perf](https://github.com/datastax/cstar_perf) - Apache Cassandra performance testing platform.
- [Spark Cassandra Stress](https://github.com/datastax/spark-cassandra-stress) - Tool for testing the DataStax Spark Connector against Apache Cassandra or DSE.
- [trireme](https://github.com/o19s/trireme) - Migration tool providing support for Apache Cassandra, DataStax Enterprise Cassandra, & DataStax Enterprise Solr.
- [cqlmigrate](https://github.com/sky-uk/cqlmigrate) -  Cassandra CQL migration tool. cqlmigrate is a library for performing schema migrations on a cassandra cluster.
- [cassandra-migration-tool-java](https://github.com/smartcat-labs/cassandra-migration-tool-java) - Cassandra migration tool for java is a lightweight tool used to execute schema and data migration on Cassandra database.
- [Cassalog](https://github.com/hawkular/cassalog) - Cassalog is a schema change management library and tool for Apache Cassandra that can be used with applications running on the JVM.
- [cdeploy](https://github.com/rackerlabs/cdeploy) - Cdeploy is a simple tool to manage your Cassandra schema migrations in the style of dbdeploy.
- [Web: Cassandra Calculator](https://www.ecyrd.com/cassandracalculator/) - Simple calculator to see how size / replication factor affect the system's consistency.
- [Cassandra-web](http://avalanche123.com/cassandra-web/) - Web interface for Apache Cassandra.
- [CassanddraRestfulAPI](https://github.com/rohitsakala/CassandraRestfulAPI) - CassandraRestfulAPI project exposes the cassandra data tables with the help of Restful API.
- [Netflix: Staash](https://github.com/Netflix/staash) - Language-agnostic as well as storage-agnostic web interface for storing data into persistent storage systems, the metadata layer abstracts a lot of storage details and the pattern automation APIs take care of automating common data access patterns.
- [cql-vim](https://github.com/elubow/cql-vim) - Cassandra CQL Syntax Highlighter for Vim.
- [Presto](https://prestodb.io/) - Distributed SQL Query Engine for Big Data. Presto allows querying data where it lives, including Hive, Cassandra, relational databases or even proprietary data stores.
- [SSTable Tools](https://github.com/tolbertam/sstable-tools) - Toolkit for parsing, creating and doing other fun stuff with Cassandra 3.x SSTables.
- [Cassandra-Exporter](https://github.com/masumsoft/cassandra-exporter) - Simple Tool to Export / Import Cassandra Tables into JSON.
- [Cassandra SStable Tools](https://github.com/instaclustr/cassandra-sstable-tools) - Multiple different tools combined into one that helps admins get summaries, metadata, partition info, cell info.
- [Cassandra-Client](https://github.com/Kindrat/cassandra-client) - Simple gui tool for browsing tables and data in Cassandra.
- [CQL Data Modeler](https://www.sestevez.com/sestevez/CassandraDataModeler/) - Very useful tool to test out a CQL schema and visualize what the partition would like in relationship to the columns and rows.
- [Cassandra Snapshot Backup](https://github.com/avinash-mishra/cassandra_snapshot_backup) - Quick and easy way to snapshot files in a Cassandra database and back them up using Ansible.
- [Slothsandra](https://github.com/MacKittipat/slothsandra) - Integration for Cassandra with the Slack app, which stores old messages that Slack no longer does itself.
- [sandraREST](https://github.com/aksakalli/sandraREST) - Cassandra manager with a web UI for RESTful APIs.
- [Cassandra Leadership](https://github.com/paradoxical-io/cassandra.leadership) - Library to help elect leaders using cassandra. Uses paxos to build a leadership election module.
- [Terraform Cassandra](https://github.com/conrad-mukai/terraform-cassandra) - Terraform module that creates a Cassandra cluster.
- [Datadog](https://www.datadoghq.com/blog/monitoring-cassandra-with-datadog/) - Third party tool that allows monitoring and metrics for Cassandra nodes and clusters.
- [tlp-cluster](http://thelastpickle.com/tlp-cluster/) - Provisioning tool for Apache Cassandra designed for developers looking to benchmark and test Apache Cassandra. It assists with builds and starting instances on AWS.
- [Helenos](https://github.com/tomekkup/helenos) - Free web based environment that simplifies a data exploring & schema management with Apache Cassandra database.
- [ValuStor](https://github.com/Sensaphone/ValuStor) - ValuStor is a key-value pair database solution.
- [Cassandra-Migration](https://github.com/hhandoko/cassandra-migration) - Apache Cassandra / DataStax Enterprise database migration (schema evolution) library.
- [JanuesGraph-Utils](https://github.com/IBM/janusgraph-utils) - Tool to Develop a graph database app.
- [Scylla-Migrator](https://github.com/scylladb/scylla-migrator) - Migrate data extract using Spark to Scylla, normally from Cassandra.
- [Cassandra CA Manager](https://github.com/eevans/cassandra-ca-manager) - Create and sign Java keystores.
- [Zipkin](https://github.com/openzipkin/zipkin) - Distributed tracing system.
- [Instaclustr Kerberos plugin](https://github.com/instaclustr/cassandra-kerberos) - GSSAPI authentication provider for Apache Cassandra.
- [Instaclustr Java Driver for Kerberos](https://github.com/instaclustr/cassandra-java-driver-kerberos) - GSSAPI authentication provider for the Cassandra Java driver.
- [Instaclustr Minotaur](https://github.com/instaclustr/instaclustr-minotaur) - Command line tool for consistent rebuilding of a Cassandra cluster.
- [Instaclustr TTL Remover](https://github.com/instaclustr/cassandra-ttl-remover) - Command line tool for rewriting SSTables to remove TTLs.
- [Instaclustr SSTable Generator](https://github.com/instaclustr/cassandra-sstable-generator) - CLI tool for programmatic generation of Cassandra SSTables.
- [Instaclustr Exporter](https://github.com/instaclustr/cassandra-exporter) - Java agent that exports Cassandra metrics to Prometheus.
- [Instaclustr Go Client for Instaclustr Icarus](https://github.com/instaclustr/instaclustr-icarus-go-client) - Go client for Instaclustr Icarus sidecar.
<!-- Website currently down 4/19/21 - [KDM by Datafluent](https://www.datafluent.org/) - KDM is a big data modeling tool specialized for Apache Cassandra which allows you to go through the query driven methodology to go from a conceptual data model to an optimized physical data model. -->
<!-- double-link - [Express-Cassandra](https://github.com/masumsoft/express-cassandra) - Cassandra ORM/ODM/OGM for Node.js with Elassandra & JanusGraph Support. -->
<!-- double-link - [Instaclustr Esop](https://github.com/instaclustr/esop) - Swiss knife for backup and restore of your node to GCP, Azure, S3, Ceph etc. Supports backup and restoration of commit logs too. Esop is embedded in [Instaclustr Icarus](https://github.com/instaclustr/icarus) sidecar so you may backup and restore your cluster remotely and on-the-fly with any disruption. -->
<!-- double-link - [Instaclustr LDAP Authenticator](https://github.com/instaclustr/cassandra-ldap) - LDAP Authenticator for Apache Cassandra. -->
<!-- double-link - [Hackolade: Datamodeling for noSQL Databases](https://hackolade.com/) - Although not specialized for Cassandra, Hackolade is a general data modeling tool for noSQL databases including Cassandra, and hence Scylla, Cosmos, etc. -->

### Open Source Applications

- [Twissandra](https://github.com/twissandra/twissandra) -Twissandra is an example project, created to learn and demonstrate how to use Cassandra. Running the project will present a website that has similar functionality to Twitter.
- [ChronoServer](https://github.com/cyngn/ChronoServer) - Test server for sampling how long it takes mobile & web clients to make various types of requests to a server doing common request patterns.
- [Cassandra Cluster Admin](https://github.com/sebgiroux/Cassandra-Cluster-Admin) - Cassandra Cluster Admin is a GUI tool to help people administrate their Apache Cassandra cluster.
- [Cassandra-Tools](https://github.com/CrowdStrike/cassandra-tools) - Python Fabric scripts to help automate the launching and managing of cluster testing on AWS.
- [Cassandra Opstools](https://github.com/spotify/cassandra-opstools) - Generic scripts to review and monitor cassandra, from Spotify.  
- [CCM: Cassandra Cluster Manager)](https://github.com/pcmanus/ccm) - Script/library to create, launch and remove an Apache Cassandra cluster on localhost.
- [Netflix-Priam](https://github.com/Netflix/Priam) - Co-Process for backup/recovery, Token Management, and Centralized Configuration management for Cassandra.
- [CStar](https://github.com/spotify/cstar) - Apache Cassandra cluster orchestration tool for the command line.
- [CMB](https://github.com/Comcast/cmb) - Highly available, horizontally scalable queuing and notification service compatible with AWS SQS and SNS.
- [CassieQ](https://github.com/paradoxical-io/cassieq) - Distributed queue built off of Cassandra.
- [Cherami](https://eng.uber.com/cherami/) - Distributed, scalable, durable, and highly available message queue system.
- [Scheduler](https://github.com/PagerDuty/scheduler) - Scala library for scheduling arbitrary code to run at an arbitrary time.
<!-- double-link - [Newts](http://opennms.github.io/newts/) - A time-series data store based on Apache Cassandra. This is part of the OpenNMS family of products that are used to monitor systems. -->
<!-- double-link - [FiloDB](https://github.com/filodb/FiloDB) - High-performance distributed analytical database + Spark SQL queries + built for streaming.  -->

### Logging /Metrics

- [cassandra-log4j-appender](https://github.com/datastax/cassandra-log4j-appender) - Cassandra appenders for Log4j.
- [Metrics Collector for Apache Cassandra](https://github.com/datastax/metric-collector-for-apache-cassandra) - Metric collection and Dashboards for Apache Cassandra (2.2, 3.0, 3.11, 4.0) clusters. Comes with dashboards for Graphana.
- [Cassandra Log Tools](https://github.com/erickramirezDSE/cass_log_tools) - Simple scripts for working with Apache Cassandra logs.
- [Cassandra CFStats to CSV Parser](https://github.com/jlacefie/cfstats-csv-parser) - Converts the output of CFStats to CSV.
- [Cassandra Nagios](https://github.com/causes/cassandra-nagios) - Perl Based scripts to get metrics for monitoring using Jolokia.
- [ctop](https://github.com/pixonic/ctop) - This is a very simple console tool for monitoring column families read/write activities at remote cassandra host.
- [Cassandra StatD Agent](https://github.com/lookout/cassandra-statsd-agent) - Java Agent for Cassandra integration with StatsD.
<!-- 404 moved or made private - [Cassandra Scripts](https://github.com/bart613/cassandra) - Python based cassandra ops scripts to monitor cfstats. -->

## Resources

### Documentation

- [Apache Cassandra Documentation](http://cassandra.apache.org/doc/) - Definitive documentation for all published versions.
- [DataStax Documentation](http://docs.datastax.com/en/landing_page/doc/landing_page/current.html) - Documentation and Drivers from DataStax.

### Books

- [Cassandra: The Definitive Guide, 3rd Edition](https://www.amazon.com/gp/product/1098115163/)
- [Cassandra: The Definitive Guide, 2nd Edition](https://www.amazon.com/gp/product/1491933666/)
- [Cassandra High Availability](https://www.packtpub.com/big-data-and-business-intelligence/cassandra-high-availability)

### Courses

- [DataStax Academy](https://academy.datastax.com/) - Free online courses on Cassandra.

### Communities

- [Apache Cassandra Users Mailing List](http://www.mail-archive.com/user@cassandra.apache.org/)
- [Apache Cassandra Developers Mailing List](http://www.mail-archive.com/dev@cassandra.apache.org/)
- [Apache Cassandra Commits Mailing List](http://www.mail-archive.com/commits@cassandra.apache.org/)
- [Apache Software Foundation Slack](https://s.apache.org/slack-invite) - The #cassandra and #cassandra-dev channels are official slack channels migrating from IRC.
- [Datastax Academy Slack](https://academy.datastax.com/slack)
- [Cassandra Slack](https://cassandra-slack.herokuapp.com/)
- [Stack Overflow: Cassandra](https://stackoverflow.com/questions/tagged/cassandra)
- [Stack Overflow: cql](https://stackoverflow.com/questions/tagged/cql)
- [Stack Overflow: spark-cassandra-connector](https://stackoverflow.com/questions/tagged/spark-cassandra-connector)
- [Quora: Cassandra](https://www.quora.com/topic/Cassandra-database)
- [Meetups: Cassandra](https://www.meetup.com/topics/cassandra/?_cookie-check=mHgLvBy3N6Cke1RU)

### Blogs

- [Datastax](https://www.datastax.com/blog)
- [Codecentric: Cassandra](https://blog.codecentric.de/en/tag/cassandra/)
- [Pythian: Cassandra](https://blog.pythian.com/technical-track/cassandra-2/)
- [Instaclustr](https://www.instaclustr.com/blog/)
- [Altheroot:Cassandra](https://blog.alteroot.org/categories/cassandra/index.html)
- [OpenCredo:Cassandra](https://opencredo.com/tag/cassandra/)
- [DOAN DuyHai's Blog: Cassandra](http://www.doanduyhai.com/blog/?cat=57)
- [Amy Tobert](https://tobert.github.io/)
- [Christopher Batey: Cassandra](http://batey.info/cassandra.html)
- [Distributed Bytes:Cassandra](https://distributedbytes.timojo.com/search/label/cassandra)
- [The Netflix Tech Blog](https://medium.com/netflix-techblog)
- [Spotify R&D / Engineering Blog : Apache Cassandra](https://engineering.atspotify.com/tag/apache-cassandra/)
- [Ryan Svilha](https://lostechies.com/ryansvihla/tags)
- [Anant](https://blog.anant.us/)
<!-- 404 - [Datastax Academy](https://academy.datastax.com/developer-blog) -->

### Videos

- [Best Practices for Running Cassandra on AWS](https://www.youtube.com/watch?v=IuJldwJLyFM) - Joint webinar between Amazon Web Services (AWS) and Stackdriver, an AWS Technology partner, to learn best practices that apply to storing, analyzing and managing queries that equate to over 1+ billion measurements a day.
- [Monitoring Cassandra: Don't Miss a Thing (Alain Rodriguez, The Last Pickle) | C* Summit 2016](https://www.youtube.com/watch?v=Q9AAR4UQzMk) - In this talk Alain Rodriguez, Consultant at The Last Pickle, will discuss what to monitor in Apache Cassandra, how, and why.
- [Tuning the Spark Cassandra Connector](https://www.youtube.com/watch?v=cKIHRD6kUOc&feature=youtu.be) - Great talk by Russell Spitzer maintainer of the Spark Cassandra connector.
- [Cassandra.Lunch](https://github.com/Anant/Cassandra.Lunch) - Collection of all past Cassandra.Lunch webinars including videos, slides, and blogposts surrounding all topics Cassandra.
<!-- Redirects to datastax.com/dev- [GumGum: Multi-Region Cassandra in AWS](https://academy.datastax.com/resources/Multi-Region-Cassandra-in-AWS) -->

### Slides

- [Cassandra DataTables Using Restful API](https://www.slideshare.net/SimranKedia2/cassandra-datatables-using-restful-api) - How to create a performant API using Python / Flash.
- [HAPI Cassandra](https://github.com/victorcouste/hapi-cassandra) - Simple REST API with hapi Node.js framework on top of a Apache Cassandra database.
- [GumGum: Multi-Region Cassandra in AWS](https://www.slideshare.net/planetcassandra/gumgum-multiregion-cassandra-in-aws) - Presentation that details how Gumgum scaled out from one local Cassandra datacenter to a multi-datacenter Cassandra cluster and all the problems they encountered and choices they made while implementing it.
- [Hardening cassandra for compliance or paranoia](https://www.slideshare.net/zznate/hardening-cassandra-for-compliance-or-paranoia) - Includes details on configuring SSL, setting up a certificate authority and creating certificates and trust chains for the JVM.
- [Securing Cassandra](https://www.slideshare.net/planetcassandra/securing-cassandra-the-right-way) - Ben Bromhead CTO of Instaclustr, will explore the various ways in which you can setup and secure Cassandra appropriately for your threat environment.
- [Tuning the Spark Cassandra Connector](https://www.slideshare.net/DataStax/maximum-overdrive-tuning-the-spark-cassandra-connector-russell-spitzer-datastax-c-summit-2016) - Slides by Russell Spitzer maintainer of the Spark Cassandra connector.
<!-- awesome-lint double link error. - [CQL: This is not the SQL you are Looking For](https://www.slideshare.net/aploetz/cql-this-is-not-the-sql-you-are-loooking-for) -->
