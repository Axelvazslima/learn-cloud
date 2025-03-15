# Amazon Relational Database Service (RDS)

## What does Amazon RDS do?

Distributed relational database managed service. Cloud--based and designed to simplify the setup, operation and scaling of relational dbs.

Administrative processes like patching, backing up databases and enabling point-in-time recovery are managed automatically.

## What problems does it solve?

Purchasing a database with the right size. You can scale it based of your needs.

## Benefits

Easy to administer -> No need for infrastructure provisioning, installing and maintaining a db software.

Fast and supportive for the most demanding db applications.

You can run it in Amazon VPC -> isolate db instances or connect your db instances to existing IT infrastructure through a VPN.

## Architecting a solution

 Build for fault tolerance -> Configure it for Multi-AZ deployment. Place your master RDS instance in one AZ and a standby replica of it in another AZ. The main failed? The replica is the new main.

## Usage of Amazon RDS

### Web and mobile applications

Very large scale, hight thoughput, massive storage scalability and high availability -> and room for future growth.

### Ecommerce applications

Flexible, secured, highly scalable and low-cost db for online sales and retailing.

Help with payment card industry (PCI) compliance and focus on building high quality customers experiences.

### Mobile and online games

High throughout and availiability.

No need for provisioning, scaling or monitoring db servers.

## What else to keep in mind?

It is fully managed -> automates the maintence and security of the db instance.

Want to have access to the db OS, then get an EC2 instance and host your own database -> You are responsible for basically everything now.

## Costs

Pay-only-for-what-you-use model with no minimun fee.

On-Demand and Reserved Instances are also options.
