# AWS Global Infrastructure

Some event prevents the customers to get the wanted service? There are chains of datacenters divided into groups -> Region

> High availability, no matter the tragic circunstance.

You don't need to have datacenter(s) -> Buy hardware resources On-Demand.

Build datacenters in large groups, called Regions.

# Region

Large group of datacenters.

Through the globe, AWS builds datacenter near where the traffic is.

Inside each Region, we have multiple datacenters.

High speed fiber network.

Each Region is isolated from each other. No data goes from one to another, without you explicitly telling it to do so.

Regional data sovereign -> Part of critical design of AWS Regions.

> Data is subject to the local laws.

## Which Region do you pick?

4 business factors

    1. Compliance -> Region must live in the London Region, for example. Not all companies have location-specific data regulations.

    2. Proximity -> How close you are to your customers base (speed / latency).

    3. Feature Availabilty -> No all Regions have all features, maybe you need a feature that is in a Region that is far from your customers.

    4. Pricing -> Pricing differs based on your region, even with the same hardware (tax and etc).

## Availability Zone

Don't run your application in a single building. If a disaster happens, have a backup.

```sh
Single data center or a group of data centers within a Region.
```

Each Region consists of multiple (usually 3, but can be more) isolated AZs.

AZs are built distant to each other even in the same region - preventing natural disasters.

## What happens in case of a disaster?

Running a EC2 instance only run in one AZ. Solution to protecting it? Run multiple EC2 instances in differente AZs.

Run across at least two Availability Zones in a Region -> Your application keeps running in case of a disaster.

### Elastic Load Balancer (ELB)

Regional construct that runs across all AZs in that region communicating with EC2 instances -> Regionally Scopped Service.

## Regionally Scopped Service

Any service listed as a Regionally Scoped Service works just like ELB with no additional charges.


