# Monolithic Applications And Microsservices

Diferent ways of architecting applications.

Applications are made of multiple components and they have o communicate with each other to transmit data, fulfill requests and keep the application running.

## What are components?

It can be a lot of stuff, such as databases, UIs, business logic and etc.

## Monolithic application

If a single component fails, the whole application falls apart.

> Tightly Coupled Application.

```sh
To help maintain application availability when a single component fails, use the microsservices approach to architect your application.
```

## Microsservices

> Loosed Coupled Application

If a single component fails, it won't compromise the whole application. The other components will keep working.

Microsservice approach with services and components that fulfill different functions.

Two services facilitate application integration: Amazon SNS and Amazon SQS. Know more about them in the messaging and queing file.


