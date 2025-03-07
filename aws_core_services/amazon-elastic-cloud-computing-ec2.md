# Amazon Elastic Cloud Computing (EC2)

## What does Amazon EC2 do?

Web service that provides secure, resizable compute capacity in the cloud.

Web-scale cloud computing easier for developers.

Complete control of your computing resources and you can run it on the proven computing environment of Amazon.

## What problem does it solve?

No need for predicting upfront needs.

```sh
Scale up and down as you need to.
```

## Benefits

Provision an EC2 instance in as little as 5 minutes -> Select right CPU, storage and OS for your needs.

Change the volume size and instance type without terminating the instance.

Scale up and down to meet seasonal needs -> No need for extra servers for a few months of the year.

## Architect a solution

Multi-tier application.

Create an instance in a public subnet that hosts a website with a security group that allows internet traffic in and out. Then, create another instance that hosts a database in a private subnet with a hardened security group -> This security group restricts internet traffic, but allows the website instance to access the database instance.

## How can I use Amazon EC2?

### Host multi-tier applications

Security groups. Control the kind of acces that can reach your instances.

### Back up and disaster recovery.

Create a back up instance if your main instance fails. Scale them up until the main instances are back online -> scale them down afterwards.

```sh
Backup for clod or on-premises instances
```

### On-demand computing

Provision instances to perform computing jobs and terminate them when you are done -> save a lot of money (temporary demand).

### Host databases

AWS offers fully managed and serverless database services. However, you don't have acces to the system's OS. If you need it, you can host your own db on an EC2 instance.

### What else to keep in mind?

If you stop an instance, the Amazon Elastic Block Store (Amazon EBS) volume that is attached will retain your data. You will still be charged for that volume.

Terminate the instance and all your data on the volume will be deleted -> the volume returns to AWS for available use to other AWS customers.

## Costs

Three main price models.

### On-demand instances

Pay for the instances for the amount of time you need them. No long-term commitment or upfront.

```sh
Short term computing workloads that can not be interrupted.

Users that need low-cost computing without any upfront or long-term commitment.
```

### Spot instances

Take advantage of unused Amazon EC2 capacity in the AWS cloud for a discount -> save up to 90% compared to On-Demand prices.

Submit a request with the instance specsifications and the maximum price that you are willing to pay per hour -> Spot instance available at your submitted price = you have access to the instance.

```sh
Workloads that can be paused and restarted when computing prices meet your budget for Spot Instances.
```

### Reserved instances

Significative discount: Up to 75% compared to On-Demand prices.

You commit to paying for the instance for 1 or 3 years.

```sh
Computing needs with a steady amount usage of up to 1 year or more.
```


