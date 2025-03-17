# Amazon Relational Database Service (RDS)

## Relational Database

```sh
Relational databases are databases that stores data related to other pieces of data.
```

It uses Structured Query Language (SQL) to store and query data.

Easily understandable, consistent and scalable way.

## Relational Database Service (RDS)

It enables you to run relational databases in the AWS Cloud.

```sh
It is a managed service that automates tasks such as hardware provisioning, database setup, patching and backups.
```

You can combine it with other AWS services to fulfill your business and operational needs, like AWS lambda to query your database from a serverless application.

It offers different security options -> encryption at rest (protecting data while it is stored) and encryption in transit (protecting data while it is being sent and received).

### Amazon RDS database engines

It is availale in six databases engines, which optimizes for memory, performance or input/output (I/O)

> Amazon Aurora, PostgresSQL, MySQL, MariaDB, Oracle Database, Microsoft SQL Server.

### Amazon Aurora

```sh
It is an Enterprise-class relational database that is compatible with MySQL and PostgresSQL.
```

It is up to *5x faster than MySQL databases* and up to *three times faster than PostgresSQL databases*.

It helps you reduce your database costs by reducing unnecessary I/O operations, while ensuring that your database resources remain reliable and available.

If your workload requires **high availability**, you should consider it -> it replicates six copies of your data accross three AZs and continuously backs up your data to Amazon S3.
