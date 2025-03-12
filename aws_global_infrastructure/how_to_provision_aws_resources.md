# How to provision AWS resources

APIs.

In AWS, everything is an API call.

Three determinant ways for you to communicate with an AWS service -> invoke/call them to provision, configure and manager your AWS resources.

AWS Management Console, AWS Command Line Interface (CLI), AWS Software Development Kits (SDKs) and various other tools -> call AWS APIs.

## AWS Management Console

Test environments.

View AWS bills and monitoring.

Work with non-technical resources.

Point and click style.

## AWS Command Line Interface (CLI)

Up and running in a production type of environment.

Make API calls using the terminal on your machine.

Not a visual navigation style.

You can schedule scripts -> Automation is key to having a successful and predictable cloud deployment overtime.

Automate the actions that your services and applications perform through scripts.

Available for Windows, Mac and Linux.

## AWS Software Development Kits (SDKs)

Interact with AWS resources form various programming languages.

Use them in your programs.

No need to use low-level APIs.

Documentation and sample codes available for each supported programming language. Examples: C++, Java, .NET and more.

## Provision a resource

Log in to the AWS Management Console, write commands or write programs.

## AWS Elastic Beanstalk

Serice that helps you provision Amazon EC2-based environments.

No need to use the console or to run commands to build out EC2 instances, scaling, your network and Elastic Load Balancers.

Provide your application code and desired configurations to this service -> it takes it and build your environment for you.

Save environment configurations.

Don't focus on the infrastructure, it handles it for you.

Tasks it handles: Adjust capacity, load balancing (ELB), automatic scaling (EC2 Auto Scaling) and application health monitoring.

## AWS Cloud Formation

Create automated and repeatable deployments.

Infrastructure as code tool.

Provide it with JSON and YAML text-based documents called CloudFormations templates.

Say what you want and it handles it for you.

Not just limited for EC2-based solutions -> storage, database, analytics, machine learning and etc.

It manages all the calls to the backend AWS APIS for you.

Run the same template across multiple counts or Regions and identical environments across them will be created -> less room for human error (totally automated process).

It rolls back changes automatically if it detects errors.
