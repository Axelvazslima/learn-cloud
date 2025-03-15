# Amazon Simple Notification Service (SNS)

## What does it do?

Web service that makes it easy to set up, operate and send notifications from the cloud.

Highly scalable, flexible and cost-effective capability to publish messages from an application and immediately deliver them to subscribers (notification recipients or other applications)

## What does it solve?

Appropriate subscribers ot getting important information that they should be aware of, as events occur in their application or infrastructure.

## Benefits

Differents types of notifications across 200 countries.

Message durability -> Unavailable endpoint? It initiates a message retry policy to resend the message.

## Architecting a solution

EC2 instance fails -> CloudWatch -> (EC2 Auto Scaling -> Resized EC2 instance), (SNS -> notification sent to the appropriate subscribers, so they can investugate the issue further))

## Usage

It creates topics, or access points that identifies a specific subject or event type.

### Standard

Application can process messages that arrive more than once and out of order. It can be two types.

```sh
Fraud detection, tax calculation, critical alerting systems...
```

### FIFO

First-in-first-out

The orer of operations and events matter and duplicates are not tolerated.

```sh
Bank transaction logging, stock monitorung, flight tracking, inventory management, price update systems...
```

## What else to keep in mind?

It can't automate messages by itself -> must work together with another service, like CloudWatch or AWS Lambda.

## Costs

No upfront fees, no requirement commitments and no long-term contracts.

Pay-for-what-you-use, based on the type of topic that is used.
