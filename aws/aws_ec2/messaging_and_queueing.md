# Messaging and Queueing

```sh
Placing messages into a buffer.
```

Applications send messages to each other to communicate.

> Tightly coupled architecture: If a single component fails or changes, the whole app see the damage.

> Loosely coupled architecture: ***More reliable architecture***. If one component fails, it won't cause cascading failures. Isolated.

```sh
Application A --> Messaging Queue [messages...] --> Application B
```

The queue works as a first in first out system, must remember that.

## Amazon Simple Queue Service (SQS)

> Message queueing service.

Send, store and receive messages between software components at any volume without losing messages or requiring other services to be available.

Payload: Data contained within a message -> protected until delivery.

Amazon SQS Queues: Where messages are placed until they are processed.

## Amazon Simple Notification Service (SNS)

Can send message and notifications.

Works differently than SQS -> publish/subscribe or pub/sub model.

> Publish/subscribe service.

### Amazon SNS topic

A channel for messages to be delivered.

Configre subscribers to that topic and deliver messages to that subscribers -> one message to a topic.

The subscribers can also be endpoints, like AWS Lambda. Or they can be, email addresses, fucntions or several other options.

Can send notifications to end users by SMS, email...


