# AWS Lambda

## What does it do?

Serverless compute service that you can use to run function code tithout provisioning or managing servers.

Any type of application or backend service.

Upload the code as a .zip file or container image and Lambda takes care of the rest -> run and scale it with high availability.

## What problems does it solve?

It removes all administration for apps or backend services.

You can set up your code to automatically trigger from over 200 services and SaaS apps or call it directly from any web or mobile app.

## Benefits

Serverless. Run your code without requiring you to provision or manage infrastructure.

Built-in continuous scaling that scales your app by running code in response to each event.

## Architecting a solution

User -> S3 A -> AWS Lambda -> SNS -> notification

^------ S3 B <---|

## Usage

### Web Applications

### Data processing

AWS services -> Amazon S3, DynamoDB, Kinesis, Amazon SNS and CloudWatch or orchestrated into workflows by AWS Step Functions.

### Real-time file processing

Process data immeditaly after an upload.

Connect to an existing Amazon Elastic File Systrem (EFS) directly -> massively parallel shared access for large-scale file processing.

### Real-time stream processing

Process real-time streaming data for application acticity tracking, transaction order processinf and click stream analysis. Or data cleansing, metrics generation, log filtering, indexing, social media analysis and IoT device telemetry and metering.

## What else to keep in mind?

It has a 15-minute limite on its runtime for each invocation.If that's not enough for your computing needs, use an EC2 instance instead.

## Costs

Pay for what you use.

Charged based on the number of requests for your lambda functions and the duration (time for the code to run).

Always free usage -> 1M requests per month and 400,000 GB-seconds of compute-time per month.

No charge is incurred when your code is not running.
