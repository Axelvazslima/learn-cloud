# Subnets and Network Access Control Lists

## Subnets

```sh
A subnet is a section of a Virtual Private Cloud (VPC) where you can group resources based on security or operational needs.
```

It can be private or public.

[AWS [VPC [[public subnet with Amazon EC2 instances] <--> [private subnet with databases]]]]

Public subnets -> It contains resources that need to be accessed by the public.

Private subnets -> It contains resources that need to be hidden form the public. Only accessible through your private network.

In a VPC, subnets can communicate with each other: Check the wanna-be diagram.

## Network traffic in a VPC

When a customer requests resources from an application hosted in the AWS Cloud, this request is sent as a **packet**.

```sh
A packet is a unit of data sent over the internet or a network.
```

The request enter into a VPC through an internet gateway. Before a packet can enter into a subnet or exit from it, it checks for permissions (who sent the packet and how the packet is trying to communicate with the resources in a subnet).

The VPC components that checks packets permissions for subnets is a **Network Access Control List**.

## Network Access Control List (Network ACL)

```sh
Virtual firewall that controls inbound and outbound traffic at the subnet level.
```

Each AWS account inscludes a default network ACL and when creating your own VPC, you can use your default Network ACL or create a custom one.

Your default Network ACL is set to allow all inbound and outbound traffic , but you can modify it and add your own rules.

For custom created Network ACLs, all inbound and outbound traffic is denied by default -> add rules to specify which traffic to allow.

All Network ACLs have an explicit deny rule -> if a packet doesn't match any of the other rules on the list, the packet is denied.

Network ACL <--> [public subnet]

### Stateless packet filtering

Network ACLs perform stateless packet filtering -> they remember nothing and check packets that cross the subnet borders each way (inbound and outbound).

```sh
The VPC component that checks packets permissions for an Amazon EC2 instance is a security group.
```

### Stateful packet filtering

```sh
Security Groups perfor stateful packet filtering. They remember previous decisions made for incoming packets.
```

> Made for instances.

The key difference between Security Groups and Network Access Control List (ACLs) is that Securoty Groups are stateful and ACLs are stateless.

## VPC component recall

Private subnet -> isolate databases containing customers' peronal informations.

Virtual private gateway -> create a VPN connection between the VPC and the internak corporate network.

Public subnet -> subnet that the customers must have access to. Internet access.

AWS Direct Connect -> estabilish a dedicated connection between the on-premises data center and the VPC.
