# AWS Identity And Access Management (IAM)

## What does IAM do?

Centralized security management system that is included in every AWS account to control identity access to AWS services -> Which services each identity can access and the kind of actions the identity can perform.

### User

It is an entity you create in AWS that represents the person or service who uses it to interact with AWS.

### Group

Collection of IAM users.

```sh
Specify permissions.
```

### Role

Identity with permissions policies attached to it.

IAM user can assume these policies to temporarily take on different permissions for a specific task.

## What problems does it solve?

Users have more acces than they should.

Principle of least privilege -> You only have access to something if you it was explicitly granted to you.

## Benefits

Simple user interface -> easy to manage accesses.

Many system-generated policies, but you can also create new ones.

## Architecting a solution

A user in the dev account is assuming a role in the production account. The role returns a temporary security credential -> temporary access to the aws service based on the policy that is attached to the role.

## Usage

### Fine-grained control

AWS service APIs, sprecific resources and conditions (based on IP address). Using Secure Sockets Layer (SSL) or wether they have authenticated with a multi-factor auth device.

### Multi-factor authentication (MFA)

Protect your AWS environment using MFA -> no extra costs and augments user name and password credentials.

Physical possesion of a hardware MFA or MFA-enabled mobile device using a valid MFA code.


### Analyze access

Secutiry teams and administrator can quickly validate that your policies only provide the intendend public and cross-account access to your resources.

Easily identify and refine your policies to allow access to only the services that are being used -> principle of least privilege.

### Integrate with your corporate directory

Grant access to your emplyess and applications federated to the AWS Management Console and AWS service APIs.

Use any identity management solution that supports Security Assertion Markup Langage (SAML) 2.0. Or one of the AWS federtion samples, such as AWS Management Console single sign-on (SSO) or API federation.

## What else to keep in mind?

### Implicit deny

Deny user, group or role access to a specific service.

Default for all new identity created.

### Explicit allow

Overrides an implicit deny.

It can grant full or partial access -> depends on the attached IAM policy.

### Explicit deny

Deny user, groups or roles to have access to services or actions.

Similar to implicit deny, but it **can not be override** by an explicit allow.

## Costs

No additional charge. Except when you access other AWS services by using your IAM users' credential.
