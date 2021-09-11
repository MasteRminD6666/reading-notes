![](https://www.clariontech.com/hs-fs/hubfs/SQL-NOSQL.png?width=813&name=SQL-NOSQL.png)


## What is a SQL database?
A SQL database supports structured query language (SQL) — a domain-specific programming language for querying and manipulating data in a relational database. The key to the relational model is abstracting data as a set of tuples organized into “relations,” which allows for abstraction over the physical representation of data and access paths.

The "relational" in “relational database” refers to the "relational model" of data management devised by IBM researcher E.F. Codd in the early 1970s. Though SQL is not the only language used for implementing query over the relational model, it is the most popular (despite not strictly conforming to Codd's original design). Beginning with “System R,” the relational model was later popularized by subsequent database systems.

Relational databases have been the industry standard since the late 1970s, though many of their "navigational" predecessors (e.g., Apollo 11-era IMS) are still under active development. In fact, most current enterprise systems architecturally descend from the aforementioned System R.

# "NewSQL" and "Distributed SQL"
During the early 2010s, several organizations began building SQL-based systems to eliminate NoSQL limitations as well as “NoSQL vs. SQL” tradeoffs causing data inaccuracy and horizontal scalability problems.

This led to the emergence of two distinct relational database systems:

- NewSQL: Adds distributed logic to existing SQL databases with varying degrees of user transparency. Citus Data (acquired by Microsoft) and Vitess best exemplify "NewSQL"-style distributed engines.*
- Distributed SQL: Imparts a "ground-up" approach to building horizontally scalable relational databases. CockroachDB and Spanner, both designed to be more advanced than NewSQL, best exemplify “Distributed SQL”-style engines.
NOTE: A common motivation for the development of both NoSQL and NewSQL is the high cost required to build a relational database.

## SQL databases: Pros and cons
## Pros
- Flexible queries: Enables support for diverse workloads. Abstracts data over underlying implementations and allows engines to optimize queries to fit on-disk representations.
- Reduced data storage footprint: Due to normalization and other optimization opportunities, a reduced footprint maximizes database performance and resource usage.
- Strong and well-understood data integrity semantics: Atomicity, consistency, isolation and durability, or ACID, are database properties that guarantee valid transactions.
# Cons
- Rigid data models: Requires careful up-front design to ensure adequate performance and resistance to evolution. SQL has a predefined schema, so changing it often includes downtime.
- Limited horizontal scalability: It is either completely unsupported, supported in an ad-hoc way or only supported on relatively immature technologies.
- Single point of failure: Non-distributed engines are mitigated by replication and failover techniques.


# What is a NoSQL database?
Rooted in graph, document, key-value pairs and wide-column stores developed in the early 1990’s, NoSQL (“Not only SQL”) rose in the mid-2000s due to the emergence of cloud, big data, and web and mobile applications. Today it is the preferred database due to its performance quality, ability to scale and ease of use.

Research on non-relational systems (e.g., BigTable and Dynamo) led to the rise of startups and open source projects dedicated to increasing the relational model’s horizontal scalability and loosening the rigidity of its table design. Their emergence revealed a need for better designs and looser constraints for relational databases.

Though the relational database community responded to these needs with NewSQL, new databases continued to rapidly appear. As a result, multiple database systems now exist, each addressing the fundamental problem (i.e., storing bits and making them available later) in a slightly different way.

In many ways, this boom is a boon for developers. Not all applications have relational database-shaped problems or need to make the tradeoffs that relational databases impose on data and availability models. However, this flexibility does not come without a cost.

To make a good technical decision between NoSQL databases, a developer must have a thorough understanding of the full design space so the tradeoffs made by a particular system are clear. In other words, you don't want to accidentally sacrifice consistency isolation when your application actually requires it.

# NoSQL databases: Pros and cons
# Pros
- Scalable and highly available: Many NoSQL databases are designed to support seamless, online horizontal scalability without significant single points of failure.
- Flexible data models: Most non-relational systems do not require developers to make up-front commitments to data models. Existing schemas are dynamic, so they can often be changed “on the fly.”
- Dynamic schema for unstructured data: Documents can be created without a defined structure first, which enables each to have its own unique structure.  Syntax varies per database and fields can be added as you build the document.
- High performance: A limited database functionality range (e.g., by relaxing durability guarantees) enables high performance amongst many NoSQL databases.
- High-level data abstractions: Beyond the "value in a cell" data model, NoSQL systems provide high-level APIs for powerful data structures. For example, Redis includes a native-sorted set abstraction.
# Cons
- Vague interpretations of ACID constraints: Despite the widespread belief that it supports NoSQL systems, ACID interpretations can be too broad to make clear determinations about database semantics.
- Distributed systems have distributed systems problems: Though not specific to NoSQL systems, encountering such problems is common amongst NoSQL developers and may require SME troubleshooting.
- Lack of flexibility in access patterns: Without the abstraction found in relational databases, the on-disk representation of data leaks into the application's queries and leaves no room for NoSQL engines to optimize queries.
