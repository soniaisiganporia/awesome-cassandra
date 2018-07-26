# Awesome Cassandra [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome [Apache Cassandra](http://cassandra.apache.org/) packages and resources. Maintained by Rahul Singh of [Anant](http://anant.us). Feel free contact me if you'd like to collaborate on this and other awesome lists. [Awesome Cassandra](https://github.com/Anant/awesome-cassandra) , [Awesome Solr](https://github.com/Anant/awesome-solr), [Awesome Lucene](https://github.com/Anant/awesome-lucene)

## Contents

- [General](#general) 

- PROGRESS [Packages](#packages)
  - [Libraries](#interfaces)  Programming Language Specific Libs for Cassandra.
  - [Tools](#tools) Applications / Tools that work with Cassandra.
  - [Projects](#projects) Other projects that use Cassandra.
  
- PROGRESS [Resources](#resources) 
  - [Documentation](#documentation) Official / unofficial documentation. 
  - [Books](#books) Popular books about Cassandra.
  - [Tutorials](#tutorials) Step by step tutorials on Cassandra.
  - [Web Sites](#web-sites) Sites ( not blogs ) on Cassandra.
  - [Blogs](#blogs) from Cassandra experts.
  - [Videos](#videos) Videos on Cassandra.
  - [Slides](#slides) Slides on Cassandra / related technologies.

## General

### Cassandra 
- [Apache Cassandra](http://cassandra.apache.org/) Manage massive amounts of data, fast, without losing sleep.
- TODO: some articles on cassandra history 
- TODO: some articles on cassandra use cases 
- TODO: cassandra disributions


### Relational -> Cassandra
- [RDBMS to NoSQL](http://www.datastax.com/relational-database-to-nosql): Your roadmap to understanding whether NoSQL is right for you.
- [MySQL to C*](http://planetcassandra.org/mysql-to-cassandra-migration/): mysql to cassandra migration guide

### Using Cassandra
- TODO: cassandra installation tutorials in local, docker, cloud (do, aws, azure, gcp)
- TODO: compiling cassandra
- TODO: running cassandra
- TODO: using cql
- TODO: using zeppelin with cassandra
- TODO: getting data in / out of cassandra



## Packages

### Libraries
- [DataStax Java Driver](https://github.com/datastax/java-driver): A Java client driver for Apache Cassandra. 
- [DataStax C++ Driver](https://github.com/datastax/cpp-driver): A modern, feature-rich, and highly tunable C/C++ client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's native protocol and Cassandra Query Language v3. http://datastax.github.io/cpp-driver/
- [DataStax Python Driver](https://github.com/datastax/python-driver): A modern, feature-rich and highly-tunable Python client library for Apache Cassandra (2.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax Ruby Driver](https://github.com/datastax/ruby-driver) : A Ruby client driver for Apache Cassandra. This driver works exclusively with the Cassandra Query Language version 3 (CQL3) and Cassandra's native protocol.
- [DataStax NodeJS Driver](https://github.com/datastax/nodejs-driver): A modern, feature-rich and highly tunable Node.js client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax C# Driver](https://github.com/datastax/csharp-driver) A modern, feature-rich and highly tunable C# client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax PHP Driver](https://github.com/datastax/php-driver): DataStax PHP Driver for Apache Cassandra http://datastax.github.io/php-driver/
- [Achilles](http://doanduyhai.github.io/Achilles/): Achilles is an open source Persistence Manager for Apache Cassandra,with the features like Advanced bean mapping (compound primary key, composite partition key, timeUUID...),Native collections and map support,and so.
- [phpcassa](https://github.com/thobbs/phpcassa): PHP client library for Apache Cassandra
- [Caffinitas](http://caffinitas.org/mapper/): Caffinitas is an advanced object mapper for Apache Cassandra which has been especially designed to work with Datastax Java Driver 2.1+ against Apache Cassandra 2.1, 2.0 or 1.2.
- OLD - [Netflix Astyanax](https://github.com/Netflix/astyanax): Astyanax is a high level Java client for Apache Cassandra, based on Thrift protocol. Not maintained.

### Tools
- [Cassandra Reaper](http://cassandra-reaper.io/): Automated repairs for Apache Cassandra. Supports all versions. 
- [cstar perf](https://github.com/datastax/cstar_perf) Apache Cassandra performance testing platform
- [Spark Cassandra Stress](https://github.com/datastax/spark-cassandra-stress) A tool for testing the DataStax Spark Connector against Apache Cassandra or DSE
- [trireme](https://github.com/o19s/trireme): Migration tool providing support for Apache Cassandra, DataStax Enterprise Cassandra, & DataStax Enterprise Solr.
- [Web: Cassandra Calculator](https://www.ecyrd.com/cassandracalculator/): A simple calculator to see how size / replication factor affect the system's consistency.
- [Docker-Cassandra](https://github.com/nicolasff/docker-cassandra): A set of scripts and config files to run a Cassandra cluster from Docker.
- [Cassandra & Zeppelin Notebook on Docker](https://github.com/academyofdata/cassandra-zeppelin): Docker-Compose script for Cassandra + Zeppelin setup.

### With Spark
- [DataStax Spark Cassandra Connector](https://github.com/datastax/spark-cassandra-connector): This library lets you expose Cassandra tables as Spark RDDs, write Spark RDDs to Cassandra tables, and execute arbitrary CQL queries in your Spark applications.
- [Stratio Deep](https://github.com/Stratio/stratio-deep): Deep is a thin integration layer between Apache Spark and several NoSQL datastores. We actually support Apache Cassandra and MongoDB, but in the near future we will add support for sever other datastores.

### Search / Secondary Indexes 
- [Elassandra](http://www.elassandra.io/): Elassandra = Elasticsearch as a Cassandra secondary index.
- [Cassandra Lucene Index](https://github.com/Stratio/cassandra-lucene-index):  Lucene based secondary indexes for Cassandra
- OLD - [Solandra](https://github.com/tjake/Solandra): Solandra is a real-time distributed search engine built on Apache Solr and Apache Cassandra.

### Admin / Monitor
- [DataStax OpsCenter](http://www.datastax.com/what-we-offer/products-services/datastax-opscenter): Simplified management for DataStax Enterprise and Cassandra database clusters.
- [Cassandra Cluster Admin](https://github.com/sebgiroux/Cassandra-Cluster-Admin): Cassandra Cluster Admin is a GUI tool to help people administrate their Apache Cassandra cluster.
- [Cassandra StatD Agent](https://github.com/lookout/cassandra-statsd-agent): Java Agent for Cassandra integration with StatsD 
- [Cassandra Scripts](https://github.com/bart613/cassandra): Python based cassandra ops scripts to monitor cfstats. 
- [Cassandra-Tools](https://github.com/CrowdStrike/cassandra-tools): Python Fabric scripts to help automate the launching and managing of cluster testing on AWS. 
- [Cassandra Opstools](https://github.com/spotify/cassandra-opstools): Generic scripts to review and monitor cassandra, from Spotify.  
- [CCM: Cassandra Cluster Manager)](https://github.com/pcmanus/ccm): A script/library to create, launch and remove an Apache Cassandra cluster on localhost.
- [Cassandra Nagios](https://github.com/causes/cassandra-nagios): Perl Based scripts to get metrics for monitoring using Jolokia.
- [Cassandra Log Tools](https://github.com/erickramirezDSE/cass_log_tools): Simple scripts for working with Apache Cassandra logs.
- [Cassandra CFStats to CSV Parser](https://github.com/jlacefie/cfstats-csv-parser): Converts the output of CFStats to CSV. 


### Queues / Schedulers
- [CMB](https://github.com/Comcast/cmb): A highly available, horizontally scalable queuing and notification service compatible with AWS SQS and SNS
- [CassieQ](https://github.com/paradoxical-io/cassieq): A Distributed queue built off of Cassandra.
- [Cherami](https://eng.uber.com/cherami/) : Distributed, scalable, durable, and highly available message queue system.
- [scheduler](https://github.com/PagerDuty/scheduler) : A Scala library for scheduling arbitrary code to run at an arbitrary time.

### Frameworks 
- [fluxcapacitor/pipeline](https://github.com/fluxcapacitor/pipeline): End-to-End, Real-time, Advanced Analytics Big Data Reference Pipeline using Spark, Spark SQL, Spark ML, GraphX, Spark Streaming, Kafka, NiFi, Cassandra, ElasticSearch, Redis, Tachyon, HDFS, Zeppelin, iPython/Jupyter Notebook, Tableau, Twitter Algebird.


### Logging 
- [cassandra-log4j-appender](https://github.com/datastax/cassandra-log4j-appender): Cassandra appenders for Log4j

## Resources 

### Documentation 
- [Apache Cassandra Documentation](http://cassandra.apache.org/doc/) Definitive documentation for all published versions. 
- [DataStax Documentation](http://docs.datastax.com/en/landing_page/doc/landing_page/current.html) Documentation and Drivers from DataStax 

### Tutorials 
- [DataStax Academy](https://academy.datastax.com/): Free online courses on Cassandra
- [Building a Streaming Data Hub with Elasticsearch, Kafka and Cassandra](http://thenewstack.io/building-streaming-data-hub-elasticsearch-kafka-cassandra/)
- [Tuning DSE Search](http://www.datastax.com/dev/blog/tuning-dse-search) Tuning DSE Search – Indexing latency and query latency
- [How to Monitor Cassandra](https://www.datadoghq.com/blog/how-to-monitor-cassandra-performance-metrics/): A guide to help you monitor Cassandra performance and work metrics regardles of which monitoring tool you choose to use.
- [Install Cassandra and Spark](http://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html): quick user guide for integration with Cassandra and Spark
- [Building a Performant API using Go and Cassandra](https://getstream.io/blog/building-a-performant-api-using-go-and-cassandra/)
- [DataStax: Basic Rules of Data Modeling](http://www.datastax.com/dev/blog/basic-rules-of-cassandra-data-modeling)


### Troubleshooting and tuning
- [Ryan Svihla's Cassandra 2.0 checklist](https://medium.com/@foundev/my-cassandra-diagnostics-checklist-brain-dump-599a2b95b118)
- [Al's Cassandra 2.1 tuning guide](https://tobert.github.io/pages/als-cassandra-21-tuning-guide.html)
- [Secret HotSpot option improving GC pauses on large heaps](http://blog.ragozin.info/2012/03/secret-hotspot-option-improving-gc.html)
- [DSE 5.1: Tuning Java Resource](https://docs.datastax.com/en/dse/5.1/dse-admin/datastax_enterprise/operations/opsTuneJVM.html)
- [Jon Haddad: Cassandra Summit Recap - Diagnosing Problems in Production](http://rustyrazorblade.com/2014/09/cassandra-summit-recap-diagnosing-problems-in-production/)

### Blogs
- [Datastax](https://www.datastax.com/blog)
- [Codecentric](https://blog.codecentric.de/)
- [Pythian](https://www.pythian.com/blog/)
- [Instaclustr](https://www.instaclustr.com/blog/) 

### Videos 
- [Best Practices for Running Cassandra on AWS](https://m.youtube.com/watch?v=IuJldwJLyFM)

### Slides
- [Cassandra DataTables Using Restful API](https://www.slideshare.net/SimranKedia2/cassandra-datatables-using-restful-api) A case on how to create a performant API using Python / Flash.
- [HAPI Cassandra](https://github.com/victorcouste/hapi-cassandra) A simple REST API with hapi nodejs framework on top of a Apache Cassandra database  
