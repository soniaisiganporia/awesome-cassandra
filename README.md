# Awesome Lucene [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome [Apache Cassandra](http://cassandra.apache.org/) packages and resources. Maintained by Rahul Singh of [Anant](http://anant.us). Feel free contact me if you'd like to collaborate on this and other awesome lists. 

## Contents

- [General](#general)

- [Packages](#packages)
  - [Libraries](#interfaces)  Programming Language Specific Libs for Lucene.
  - [Tools](#tools) Applications / Tools that work with Lucene.
  - [Projects](#projects) Other projects that use Lucene.
  
- [Resources](#resources)
  - [Documentation](#documentation) Official / unofficial documentation. 
  - [Books](#books) Popular books about Solr.
  - [Tutorials](#tutorials) Step by step tutorials on Lucene.
  - [Web Sites](#web-sites) Sites ( not blogs ) on Lucene.
  - [Blogs](#blogs) from Lucene experts.
  - [Videos](#videos) Videos on Lucene.

## General

### Documentation 
- [Apache Cassandra](http://cassandra.apache.org/) Manage massive amounts of data, fast, without losing sleep.
- [Apache Cassandra Documentation](http://cassandra.apache.org/doc/) Definitive documentation for all published versions. 
- [DataStax Documentation](http://docs.datastax.com/en/landing_page/doc/landing_page/current.html) Documentation and Drivers from DataStax 

### Relational -> Cassandra
- [RDBMS to NoSQL](http://www.datastax.com/relational-database-to-nosql): Your roadmap to understanding whether NoSQL is right for you.
- [MySQL to C*](http://planetcassandra.org/mysql-to-cassandra-migration/): mysql to cassandra migration guide

### Distributed Processsing w/ Cassandra
- OLD [Install Cassandra and Spark](http://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html): quick user guide for integration with Cassandra and Spark

## Packages

### Libraries 
- TODO : Java
- TODO : C#
- TODO : Python
- ...

### Tools 

- [DataStax Java Driver](https://github.com/datastax/java-driver): A Java client driver for Apache Cassandra. This driver works exclusively with the Cassandra Query Language version 3 (CQL3) and Cassandra's binary protocol.
- Uses Thrift [Netflix Astyanax](https://github.com/Netflix/astyanax): Astyanax is a high level Java client for Apache Cassandra, based with Thrift protocal.
- OLD [Hector](https://github.com/hector-client/hector) : Hector is a high level Java client for Apache Cassandra, based with Thrift protocal.
- [Caffinitas](http://caffinitas.org/mapper/): Caffinitas is an advanced object mapper for Apache Cassandra which has been especially designed to work with Datastax Java Driver 2.1+ against Apache Cassandra 2.1, 2.0 or 1.2.
- [Achilles](http://doanduyhai.github.io/Achilles/): Achilles is an open source Persistence Manager for Apache Cassandra,with the features like Advanced bean mapping (compound primary key, composite partition key, timeUUID...),Native collections and map support,and so.

## Projects

### With Spark
- [DataStax Spark Cassandra Connector](https://github.com/datastax/spark-cassandra-connector): This library lets you expose Cassandra tables as Spark RDDs, write Spark RDDs to Cassandra tables, and execute arbitrary CQL queries in your Spark applications.
- [Stratio Deep](https://github.com/Stratio/stratio-deep): Deep is a thin integration layer between Apache Spark and several NoSQL datastores. We actually support Apache Cassandra and MongoDB, but in the near future we will add support for sever other datastores.

### Search Engine
- [Elassandra](http://www.elassandra.io/): Elassandra = Elasticsearch as a Cassandra secondary index.
- OLD - [Solandra](https://github.com/tjake/Solandra): Solandra is a real-time distributed search engine built on Apache Solr and Apache Cassandra.

### Admin and Monitor
- [DataStax OpsCenter](http://www.datastax.com/what-we-offer/products-services/datastax-opscenter): Simplified management for DataStax Enterprise and Cassandra database clusters.
- [Cassandra Cluster Admin](https://github.com/sebgiroux/Cassandra-Cluster-Admin): Cassandra Cluster Admin is a GUI tool to help people administrate their Apache Cassandra cluster.
- [How to Monitor Cassandra](https://www.datadoghq.com/blog/how-to-monitor-cassandra-performance-metrics/): A guide to help you monitor Cassandra performance and work metrics regardles of which monitoring tool you choose to use.

### Queues / Schedulers
- [CMB]
- [CassieQ](https://github.com/paradoxical-io/cassieq): A Distributed queue built off of Cassandra.
- [Cherami]