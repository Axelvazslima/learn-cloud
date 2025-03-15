# Amazon Simple Storage Service (S3)

## Object Storage

Each object consists of *data*, *metadata* and a *key*.

Data -> Image, video, text document or any other type of file.

Metadata -> Information about what the data is, how it is used, the object size and so on.

Key -> Unique identifier.

Different to what happens when you modify a data in EBS (back up only saves the new data), when a file storage is changed the whole object is updated.

## Amazon Simple Storage Service (S3)

```sh
Service that provides object-level storage. It stores data as objects in buckets.
```

You can upload any type of file into it.

It offers *unlimited storage space* and the maximum size for a *single file is 5TB*.

You can set permissions to control visibility and access to it. You can also use the S3 versioning to track changes to your objects overtime.

### Amazon S3 storage classes

You can choose from a range of storage classes -> fit for your business and costs.

Important factors to look to consider when choosing S3 classes:
    * *How often* you plan to retrieve your data.
    * *How available* your data needs to be.

### S3 Standard

```sh
High availability for objects and has a higher cost than other classes intended for infrequently accessed dataand archival store.
```

> Designed for *frequently accessed* data.

> Stores data in a *minimum of three Availability Zones*.

Ideal for websites, content distribution and data analytics -> wide range of use cases.

### S3 Standard-Infrequent Access (S3 Standard-IA)

```sh
Ideal for infrequently accessed data, but requires high availability when needed.
```

> Ideal for *infrequently accessed data*.

> Stores data in a *minimum of three Availabilty Zone*.

> Similar to Amazon S3 Standard, but has *lower storage price* and *higher retrieval price* -> same level of availability as well.

### S3 One Zone-Infrequent Access (S3 One Zone-IA)

> Stores data in a *single Availability Zone*.

> Has a *lower storage price than Amazon S3 Standard-IA*.

Conditions to use it:
    * *Save costs* os storage.
    * You can *easily reproduce your data* in the event of an Availabilty Zone failure.

### S3 Intelligent-Tiering

```sh
Amazon S3 monitors objects' access patterns -> didn't accessed an object in 30 consecutive days? It gets moved automatically to the infrequent access tier. But, if you access an object in the infrequent access tier, it gets automatically moved to the frequent access tier.
```

> Ideal for data with *unknown or changing access patterns*.

> Requires a *small monthly monitoring and automation fee per object*.

### S3 Glacier Instant Retrieval

> You can quickly retrieve an archived object (see how important this is for you) -> a few milliseconds (same as S3 standard).

> Ideal for datas that require immediate access.

### S3 Glacier Flexible Retrieval

```sh
Low-cost storage class that is ideal for data archiving. You can retrieve its data from 1 minute to 12 hours.
```

> Ideal for *customer records*, *older photos* and *video files*.

### S3 Glacier Deep Archive

```sh
Long-term retention and digital preservation for data that might be *accessed once or twice in a year*. All objects from this class are replicated and stored across at least three Availability Zones.
```

> *Lowest-cost* object storage class.

> Ideal for *archiving*.

> Able to retrieve data within 12 to 48 hours.

### S3 Outposts

```sh
It delivers objects to your on-premises AWS Outposts environment. It is designed to store data durably and redundantly across multiple devices and servers on your Outposts.
```

> It works well for workloads with local data residency requirements that must satisfy *demanding performance needs by keeping data close to on-premises applications*.

> It creates *S3 buckets on Amazon S3 Outposts*.

> Make it easier to *retrieve*, *store* and *access* data on AWS Outposts.
