# User Permissions And Access

AWS offers a service for managing users and their access in the cloud infrastructure.

## Amazon Identity and Acess Management (IAM)

> It enables you to manage access to AWS services and resources securely.

Configure access based on your company's specific operational and security needs -> combine IAM features.

## AWS Account Root User

> It has complete access to all the AWS services and resources in the account.

[Create AWS account] --> [Create your first IAM user and give it permission to create other users] --> [Log in as the new IAM user and continue to create users, Only access the root user for a limited number os tasks]

### Best practices

Do **not** use root user for everyday tasks -> use the root user to create your furst IAM user and assign it permissions to create other users.

Then, continue to create other IAM users and access those identities for performing regular tasks throughout AWS.

Only use the root user when you need to perform a limited number of tasks that are only available to the root user -> changing your root user email address and changing your AWS suport plan.

## IAM users

> Identity that you can create in AWS. It represents the person or application that interacts with AWS services and resources -> name and credentials.

By default, a new user has no permissions granted to it -> permissions must be granted.

### Best practices

Create individual IAM users for each person that needs to access AWS, even if multiple people need the same level of access.

## IAM policies

> Document that allows or denies permissions to AWS services and resources.

It enables you to customize users' level of access to resources -> users only access specific S3 buckets in your account.

### Best practices

> Least privilege.

Prevent users or roles from having more permissions than needed to perform their tasks.

### IAM policy example

> This piece of code allows permission to access the objects in the S3 bucket with ID: AWSDOC-EXAMPLE-BUCKET.

```code
{
    "Version": "2012--10-17",
    "Statement": {
        "Effect": "Allow",
        "Action": "S3:ListObject",
        "Resource": "arn:aws:s3:::AWSDOC-EXAMPLE-BUCKET"
    }
}
```
