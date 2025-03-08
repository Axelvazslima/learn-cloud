# Amazon DynamoDB

## What does it do?

Serverless non-relational database that can store and retrieve any amount of data and serve any level of request traffic.

Scale you db tables' throughput capacity up or down without downtime.

Use AWS Management Console to monitor resource utilization and performance metrics.

## What problems does it solve?

Offload the administrative burdens of operating and scaling a distributed database.

No need to worry about hardware provisioning, setup and configurations, replication, software patching or cluster scaling.

## Benefits

Consistent, single-digit millisecond response time t any scale.

Serverless -> No servers to provision, patch or manage and no software to install, maintain or operate.

ACID transactions -> build business-critical apps at scale. It encrypts all data by default and provides fine-grained identity and access control on all your tables.

## Architecting a solution

S3 -> App <-> API Gateway <-> AWS Lambda <-> DynamoDB

## Usage

### Retail

Free from scaling concerns and operational burdens -> key competitive advantage.

High velocity and extreme-scaled events

### Gaming

Game state, player data, session history and leaderboards.

Scale reliably to millions of concurrent users and requests while ensure consistely low latency.

### Banking

Build cloud-native apps to increase agility, reduce time to market and minimize operational overhead.

Ensure security, reliability and continued high availability of their apps.

### Ad Tech

Companies in advertising technology.

Key-value store for storing various kinf of marketing data.

User profiles, user events, clicks and visited links.

## What else to keep in mind?

### Non-relational database

Key-value pairs, documents and graphs.

Dynamic and quick to add information.

Focus on collections of documents.

It scales horizontally ny increasing servers.

```sh
Internet-scale applications, real-time bidding, shopping carts and customer preferences.
```

### Relational database

Rows and columns.

Fixed.

Structured Query Language (SQL).

Scales vertically by increasing hardware power.

```sh
Traditional applications, enterprise resource planning (ERP), customer relationship management (CRM) and e-commerce.
```

## Costs

It charges for reading, writing and storing data in its tables.

It has optional features you can enable -> more costs.

On-demand and provisioned -> each one has specific billing options for processing reads and writes on the tables.
