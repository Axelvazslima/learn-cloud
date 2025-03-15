# Amazon Virtual Private Cloud (VPC)

## What does it do?

Launch AWS resources in a logically isolated virtual network that you define.

```sh
Foundational AWS service.
```

Easy to customize your VPC's network configuration.

You can create a public-facing subnet for your web servers that have access to the internet. You can also use it to place your backend systems in a private-facing subnet with no internet access.

```sh
Multiple layers of security to help control access to Amazon EC2 instances in each subnet.

Security groups and network access control lists (network ACLs).
```

## What problems does it solve?

Increase and monitor the security for your VPC on demand.

You can cerate a datacenter when you need it and terminate it when you no longer need it.

## Benefits

Advanced security -> perform inbound and outbound filtering at the instance and subnet levels.

Simple setup -> Less time setting up, managing and validating.

Control your virtual networking environment -> Choose your IP Address range, create your own subnets and configure route tables to any available gateways.

## Achitect a solution

The public subnet has an EC2 instance that hosts a web application that has access to the internet.

The private subnet has an RDS instance that is protected from direct access to the internet.

Notebook <-> Internet <-> Internet Gateway <-> (Amazon EC2 instance - Amazon RDS instance).

## How can I use it?

### Hosting a simple website

Additional layers of securoty that the its configuration provide.

### Host multi-tier web applications

Strictly enforce access and security restrictions between your web servers, application servers and databases.

Launch web servers in a publicly accessible subnet while running your application servers and databases in private subnets -> Application servers can't be directly accessed from the internet.

### Back up and recover

Disaster recovery site at a fraction of the cost.

Periodically back up critical data from your data center to a small number of Amazon EC2 instances.

Import your VM images to Amazon EC2.

It can quickly launch replacement compute capacity in AWS.

When the disaster is over, you can send your mission-critical data back to your data center.

### Extend your corporate network

Move apps to the cloud or launch additional web servers. Add more compute capacity to your network by connecting your VPC to your corporate network.

## What else?

Create one by using a template VS Creating one from scratch.

Creating one from Scratch -> Automatically create a route table, a network ACL and a security group. Then, you configure them according to your needs.

If you must delete a VPC, be sure to terminate any EC2 or RDS instances that you have provisioned in the VPC.

## Costings

Free for basic level -> default VPC.

Many components that doesn't cost anything -> Subnets, route tables, network ACLs, security groups and an internet gateway.

You can add paid features such as NAT gateway and elastic IPs.

Also, any service that you use with it, such as Amazon EC2 can have associate costs.
