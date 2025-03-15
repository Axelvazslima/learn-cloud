# Directing Traffic With Elastic Load Balancing

```sh
Host that guides the process.
```

Multiple EC2 instances solving the same purpose -> Load balancer routes the requests to the correct EC2 instance.

## Elastic Load Balancing (ELB)

```sh
Major managed service
```

Engineered to address the undifferentiated heavy lifting of load balancing.

> Properly distributed traffic -> high performance, cost-efficient, highly available, automatically scalable.

Set and forget.

It is a *Regional Construct* -> runs at a Region level and not in the individual EC2 instance, meaning the service is automatically highly available.

```sh
Traffic --> ELB --> (EC2 instances)
```

The ELB knows when a new EC2 instance is added or when they are terminated.

```sh
Ordering Tier (frontend) --> ELB --> Production Tier (back end)
```

The ELB directs traffic to the back end that has the least outstanding requests.

> AWS service that automatically distributes incoming application traffic across multiple platforms, such as EC2 instances.

Load balancer: Single point of contract for all incoming web traffic to Auto Scaling group -> add or remove Amazon EC2 instances in response to the amount of incoming traffic, *these requests route to the load balancer first*. Then, the requestss spread across multiple resources that will handle them.

ELB and Amazon EC2 Auto Scaling are separate serices, but they work together to help ensure that applications running in Amazon EC2 can provide high performance and availability.

> Low-demand period: Less likely to have open EC2 instnaces with no requests -> because they dont need to be initiated.

> High-demand period: ELB directs the traffic to the most appropiate EC2 instance, because there is (prpbably) more than one running at the time.

Remember: Services work together, like Amazon EC2, Amazon EC2 Auto Scaling and Elastic Load Balancing.


