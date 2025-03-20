# AWS Database Migration Service (DMS)

```sh
It enables you to migrate relational and nonrelational databases and other types of data store.
```

Move data between a *source* database and a *target* database, they can the same of different types. During the migration, your source database remainsoperational, reducing downtime for any application that rely on the database.

> Example: MySQL database in an EC2 instance, or an Amazon RDS database, to an Amazon Aurora database.

## Homogenous migrations

> Example: From MySQL to Amazon RDS FOR MySQL

The process is fairly **straightforward** -> schemas are compatible.

Create a migration task with connections to the source and target databases.

## Heterogenous migration

**Two-step process**.

First: AWS Schema Conversion Tool translates the source schema and code to match the target database.

Then: Use DMS to migrate data from the source database to the target database.

## Use cases

### Development and test database migrations

Test application against production data without affecting production users.

> Migrate a copy of your production database to your dev or test environments.

### Database consolidation

Combining several database into a single database.

> You have multiples databases and want to center them in a single place.

### Continuous replication

Replicate ongoing changes.

Sending ongoing copies of your data to other target sources instead of doing a one-time migration.

> Perform continuous data replication -> disaster recovery or geographical separation.

Create redudancies of business-critical databases and data stores to *minimize downtime* and *protect against data loss*.

### Improve integrations with data lakes

> Build data lakes and perform real-time processing on change data from your data stores.

### Remove licensing costs and accelerate business growth

> Modernize to purpose-built databases to innovate and build faster for any use case at scale for one-tenth the cost.

## Benefits

1. Discover, access, convert and migrate your database analytics workloads to AWS with *automated migration*.

2. Maintain *high availability* and *minimal downtime* during the migration process with Multi-AZ and ongoing data replication and monitoring.

3. Supports *homogenous* and *heterogenous migration* from many database providers (MySQL, Oracle Server, MariaDB, PostgresSQL, MongoDB...).

4. Migrate a *terabyte-sized database* at a *low-cost, paying only for the compute resources and additional log storage* used during the migration process.
