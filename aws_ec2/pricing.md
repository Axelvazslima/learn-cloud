# Amazon Elastic Cloud Computing (EC2) Pricing

You pay only for the compute time that you use and the price differs based on use cases.

Saving ways: Spot Instance and Reserved Instance.

## On-Demand

Ideal for short term, irregular workloads, that *can't be interrupted*. No upfront costs or minimun contracts apply.

The instance run continually until you stop them and you are charged based on what you use.

```sh
Developing applications, testing applications and running applications that have unpredictable usage patterns.
```

Not recommended for a workloads that last years, because it is more expensive.

> Unpredictable usage patterns that can not be interrupted.

## Reserved Instances

Billing discount apllied to the use of On-Demand instances in your account.

Standard RI VS Convertible RI -> Both can be bought for 1 or 3 year(s). The longer, the cheaper.

### Standard Reserved Instances

Ideal if you know the EC2 instance type and size you need for your steady-state applications. Also, depends on the AWS Region.

**Instance type and size** -> E.g. m5.xlarge

**Platform description (OS)** -> E.g. Red Hat Enterprise Linux

**Tenancy** -> Default tenancy or dedicated tenancy

You can specify an AZ for your EC2 Reserved Instance -> EC2 capacity reservation. It ensures that your EC2 instance will be availbale when you need it.

> Know exactly what you need: Type, size, OS and tenancy.

### Convertible Reserved Instances

Ideal if you need to run EC2 instances in different AZs or different instance types.

Deeper dicount when you require flexibility to run your EC2 instances.

Did your Reserved Instance time ended? You can reverve it again (new one with your new configurations) or you will automatically continue using EC2 On-Demand - or terminate the instance.

> Different AZs and/or instance types.

## EC2 Instance saving plans

Reduce your EC2 costs when you **commit**. Commit to spend a certain amount hourly to an instance family and Region for a 1-years or 3-years term -> Save up to 72% when compared to On-Demand costs. Any usage beyond the determined will be charged at On-Demand rates.

> Flexibility in your EC2 usage over your commitment term.

It doesn't have a capacity reservation option, like Reserved Instances. But, you don't need to specify up front what EC2 instance type and size, OS an tenancy.

AWS Cost Explorer to take a deeper look in your EC2 usage over a specific time range and get recommendations on how to save money based on its data.

## Spot Instances

Ideal for flexible start and end times and that can withstand interruptions.

Unused Amazon EC2 computing capacity and offer cost savings at up to 90% off On-Demand prices.

You can request a Spot Instance at any time, however it may not be available. If it is, it starts immediatly; if it isn't, you will have to wait until the desired capacity becomes available. If it's running and the capacity is no longer available, your background processing job gets interrupted.

```sh
Testing applications and experimenting new apps. Quick scale during peak periods.
```

> Flexible start and end times. Can be interrupted.

## Dedicated Hosts

Physical servers with EC2 instance capacity that is ***fully dedicated to your use***.

License compliance: per-socket, per-core or per-VM software licenses.

You can purchase On-Demand Dedicated Hosts and Dedicated Hosts Reservations.

> The most expensive.
