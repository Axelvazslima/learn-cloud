# Additional Compute Services

Even though Amaozn EC2 is flexible, reliable and scalable, depending on you use case, you might need alternatives -> You need to configure and manage a lot of things.

## Serverless

You can not see or access the underlying infrastructure or instances that are hosting your application.

Focus on your application, the rest is taken of for you -> Mangement, provisioning, scaling, high availability and maintance perspective.

### AWS Lambda

```sh
Serverless compute option.
```

The service waits for the trigger -> code is ran when it is triggered.

Run code below 15 minutes -> quick processing, like web back end handling requests.

### Amazon Elastic Container Services (ECS) or Amazon Elastic Kubernets Service (EKS) 

In case you need access to the underlying infrastructure, but still want efficiency and portability.

```sh
Container orchestrating tools.
```

The containers in this case are *docker*.

Containers are package environments for your application to run.

Containers are running isolated from each other and on top of EC2 instances (the host).

Start, stop, restart and monitor containers -> container orchestration.

Cluster: Containers running in a number of EC2 instances together.


Run your containered applications on scale.

## AWS Fargate

Serverless compute platform for ECS or EKS.

## EC2 VS Computer Services

Want: Full access to OS, host traditional applications -> use Amazon EC2.

Want: Host short-running functions, service-oriented applications, event driven applications and not provisioning or managing  servers -> use AWS Lambda.

Want: Run docker conatiner-based workloads on AWS (ECS or AKS) -> EC2 = you manage; AWS Fargate = managed for you.


