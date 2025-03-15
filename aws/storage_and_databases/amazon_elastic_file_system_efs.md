# Amazon Elastic File System (EFS)

```sh
Scalable file system used with AWS Cloud services and on-premises resources. It grows and shrinks automatically when you add or remove resources. It can scale on demand to petabytes without disrupting applications.
```

Let AWS do the heavy-lifting of *scaling* and *replication*.

Multiple instances can access the data in the EFS at the same time.

True file system from *Linux*.

Automatically scales.

Regional service.

## File Storage

Multiple users (servers, users, apps...) can access files that are stored in a shared file folders.

```sh
A storage server uses block storage with a local file system to organize files and clients access data from the file path.
```

Ideal for when a *large number of services and resources need to access data at the same time.*

## Amazon Elastic Block Storage (EBS) VS Amazon Elastic File System (EFS)

### EBS

It stores data in a single Availability Zone.

To attach an Amazon EC2 instance to an EBS both must reside at the *same Availability Zone*.

It doesn't automatically scale.

### EFS

Regional service -> It stores data in and across *multiple Availability Zones*.

The duplicate storage allows you to access data concurrently from all the Availability Zones in the Region where a file system is located.

On-premises servers can access Amazon EFS using AWS Direct Connect.


