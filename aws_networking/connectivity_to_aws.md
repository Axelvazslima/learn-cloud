# Connectivity to AWS

## Virtual Private Cloud (VPC)

There are tons of customers using AWS services all over the internet. Now, imagine these customers have created EC2 instances. Without boundaries around all of these resources, network traffic would be able to flow between them unrestricted.

```sh
Amazon VPC is a networking service used to estabilish boundaries around AWS resources.
```

It enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. Within Amazon VPC, you can organize your resources into subnets.

A subnet is a section of a VPC that can contain resources, such as Amazon EC2 instances.

## Internet Gateway

To *allow public traffic from the internet to access your VPC*, you can attach an internet gateway to the VPC.

Client --> internet request --> [AWS Cloud [(Internet Gateway)VPC [subnets with Amazon EC2 instances, for example]]]

It is a connection between a VPC and the internet. Without it, no one can access the resources within your VPC.

## Virtual Private Gateway

Access private resources of a vpc.

Extra layer of protection.

It is the component that allows protected internet traffic to enter into the VPC.

Corporate data center or content router / firewall --> internet with VPN connection --> [AWS Cloud [(Virtual Private Gateway)VPC [subnet with databases]]]

It enables you to estabilish a virtual private network (VPN) connection between your VPC and a private network, such as on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC *only if it is coming from an approved network*.

## AWS Direct Connect

```sh
It is a service that lets you to estabilish a dedicated private connection between your data center and a VPC.
```

Corporate data center or content router / firewall --> [AWS Direct Connect location [customer or partner router, AWS Direct Connect endpoint]] --> [AWS Cloud [(Virtual Private Gateway)[VPC [[public subnet with Amazon EC2 instances], [private subnet with databases]]]]]

The private connection that AWS Direct Connect provides helps you to reduce costs and increase the amount of bandwith that can travel through your network.
