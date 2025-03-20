# AWS Shared Responsability Model

AWS and its customer both have responsability for the cloud and its apps.

> Treat the environment as a collection of parts that build upon each other.

AWS is responsible for some parts of your environment and the customer for others.

## Responsabilities division

> #### **Customer**: *Security <ins>in</ins> the cloud*.
>   
>   * Customer Data
>   * Platform, Applications, Identity and Access Management
>   * Operating Systems, Network and Firewall Configurations.
>   * Client-Side Encryption; Server-Side Encryption; Networking Traffic Protection

#### **AWS**: *Security <ins>of</ins> the cloud*.
>
>   * Software
>   * Compute; Storage; Database; Networking
>   * Hardware/AWS Global Infrastructure
>   * Regions; Availability Zones; Edge Locations

## Customers

People who use AWS for their apps and etc.

> Responsible for everything they put *in* the cloud.

Control what to store in AWS, which service to use, who has access to your content, how that access is granted, managed or revoked...

## AWS

> Responsible for the security *of* the cloud.

It provides, manages and controls the components at all layers of the infrastructure -> host OS, virtualization layer, physical security of the data centers from which services operates.

It should protect all the AWS global infrastructure -> Regions, Availability Zones and Edge Locations.

Physical security of data centers, hardware and software infrastructure, network infrastructure and virtualization infrastructure.

You can't visit AWS data centers, but auditors go see and check if it's secure (computer security standards and regulations).


