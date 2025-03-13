# Security Groups

## Security Groups

```sh
A Security Group controls the traffic that is allowed to reach and leave the resources that is associated with.
```

When you create a VPC, it comes with a default Security Group. You can create additional Security Groups for a VPC, each with their own inbound and outbound rules. You can specify the source, port range and protocol for each inbound rule. And, you can specify the destination, port range and protocol for each outbound rule.

There is no additional charge for using Security Groups.

### Security Group Basics

You can assign Security Group to resources created in the same VPC as the Security Group or to resources in other VPCs if using the Security Group VPC Association feature to associate the Security Group to other VPCs in the same Region. You can also assign multiple Security Groups to a single resource.

When you create a Security Group, you must provide it with a name and a description.

Security Groups are stateful (saves previous interactions data) -> oposite of stateless (each interaction is indepedent and it doesn't save previous interactions data).

Security Groups do not filter traffic destined to and from the following: Amazon DNS, Amazon Dyanmic Host Configuration Protocol (DHCP), Amazon EC2 instance metadata, Amazon ECS task metadata endpoints, license activation for Windows instances, Amazon Time Sync Service, reserved IP addresses used by default VPC router.

There are quotas on the number of Security Groups that you can create per VPC, the number of rules that you can add to each Security Group and the number of Security Groups that you can associate with a network interface.

### Best practices

Authorize only specific IAM (Identity and Access Management) principals to create and modify Security Groups.

Create the minimum number of Security Groups that you need, to decrease the risk of error. Use each Security Group to manage access to resources that have similar functions and security requirements.

When you add inboud rules for ports 22 (SSH) or 3389 (RDP) so that you can access your EC2 instances, authorize only specific IP address ranges.

Do not open large port ranges. Ensure that access through each port is restricted to the sources or destinations that require it.

Consider creating network ACLs (Access Control List) with rules similar o an additional layer of security to your VPC.

