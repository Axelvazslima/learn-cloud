# Amazon Simple Storage Service (S3)

## What does it do?

Object storage that is built to store and retrieve any amount of data from anywhere at any time.

Simple storage service that offers industry-leading durability, availability, performance, security and virtually unlimited scalability at low costs.

## Problems solved

Add as many files as you need -> stop guessing capacity.

```sh
Elastic and scales automatically to meet your storage requirements.
```

Files uploaded are automatically areplicated across multiple AZ in the Region -> high availability and durability.

## Benefits

Consistent data whenever you need it -> native cloud storage, gigh availability, performance, scalability and durability.

Highly scalable -> serverless.

Unmatched security, compliance and audit capabilities in the cloud.

## Architecting a solution

Browser <-> Internet <- Amazon CloudFront <- Amazon S3

## Usage

### Backup and restore

### Disaster recovery

### Archive

Retire physical infrastructure and archive data with Amazon S3 Glacier and S3 Glacier Deep Archive -> These two retain objects long-term at the lowest rates.

Create an S3 lifecycle policy to archive objects throughout their lifecycles, or upload objects directly to the archival storage classes.

### Data lakes and big data analytics

Build a data lake in Amazon S3 and extract valuable insights by using query-in-place, analytics and machine learning tools. As it grows, use S3 Access Points to easily configure access to your data, with specific permissions for each application or set of applications.

## What else to keep in mind?

It is designed for object storage, not block storage.

### Object storage

Meant for read-intensive files that are not written to -> if it need a change, it can be overwritten.

```sh
Pictures, videos, documents and static websites.
```

### Block storage

More structured set of data hosting that is often written to.

Amazon S3 is not designed for this -> use Amazon Elastic Block Store, instead.

## Costs

Pay-for-what-you-use.

No minimum fee.

Some prices vary across Amazon S3 Regions. Billing prices are based on the location of your Amazon S3 bucket.
