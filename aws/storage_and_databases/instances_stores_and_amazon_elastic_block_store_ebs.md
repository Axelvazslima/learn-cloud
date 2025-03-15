# Instance Stores and Amazon Elastic Block Store (EBS)

## Instance Stores

```sh
Block-level storage volumes that acts like physical hard drives.
```

It provides *temporary* block-level storage for an Amazon EC2 instance. An instance store is disk storage that is physically attached to the host computer for an EC2 instance. - and, therefore, has the same lifespan as the instance.

Amazon EC2 instance -- Instance Store with data -> instance stops -> Now an instance Store withot data (deletes all previous data).

Recommended use case -> Temporary data that you don't need in the long term.

## Elastic Block Store (EBS)

```sh
It is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. Even if you stop or terminate an instance, its data will still be available.
```

**Creation** Define the configuration (volume size and type) and provision it.

EBS contains data *needs to persist*, so it is recommended that you back up the data. You can create incremental backups of EBS volumes by creating *Amazon EBS snapshots*.

### Amazon EBS snapshots

```sh
Incremental backup for EBS volumes.
```

Only the new added data gets backed up. The first back up copies all the data. Then, only the data that changed since the last back up is copied.

It separates drive from the host computer of an EC2 instance.
