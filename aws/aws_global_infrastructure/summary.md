# Summary

Main topics on this directory: Global Infrastructure -> Regions, Availability Zones and Edge Locations (CDNs, Amazon CloudFront and AWS Outposts).

Different ways of provisioning AWS resources -> AWS Management Console, AWS Command Line Interface (CLI) and Software Development Kits (SDKs). Alongside, AWS Elastic Beanstalk and CloudFormation.

## AWS Global Infrastructure

*Region* is a geographical location where AWS datacenters are located.

Inside a Region, there are some *Availability Zones*. These AZs are isolated from each to help secure users' services to work if happens a tragedy, such as natural disasters. They are tens os miles away from each other and usually there are 3 AZs in a Region, but some Regions have more than that.

Best Practice: Deploy your infrastructure in 2 or more AZs -> Security and high availability. Some AWS services, like Amazon SNS, ELB and Amazon SQS already do this for you.

CDNs -> Copy a content from cache and save it in another Region closer to your customer to provide low latency.

Edge Locations -> Deploy content worldwide to speed up delivery (Use CDN, like Amazon CloudFront).

AWS Outposts -> Edge Device. Allow you to run AWS infrastructure in your own datacenter.

## Provisioning AWS Resources

AWS Management Console -> Graphic Interface. Point and click.

AWS Command Line Interface (CLI) -> Run AWS shell in your terminal and initiate services from there.

Software Development Kits (SDKs) -> Call AWS APIs in your code.

AWS Elastic Beanstalk -> Takes care of your infrastructure and initiate EC2 instances. You can save configurations to replicate them in another projects or another time.

AWS CloudFormation -> Takes care of the infrastructure for you. You can save your configurations to use later. *Infrastructure as code* (provide JSON or YAML files to configure it). It works for a lot of services, not only EC2 instances (storage, databases, analytics, machine learning and etc).


