# AWS Well-Architected Framework

It is designed to help you build the most secure, high-performing, resilient, efficient and const-effective infrastructure possible in the AWS Cloud.

## Five Pillars

The foundations must be solid.

```sh
< Operational Excellence <-> Security <-> Reliability <-> Performance Efficiency <-> Cost Optimization >
```

### Operational Excellence

Ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures.

```sh
Code annotating documentation, anticipating failure and frequently making small and reversible changes
```

### Security

Ability to protect your information, systems and assets while delivering business value through risk assessments and mitigation startegies.

Best practices -> Automate security best practices when possible, apply security at all layers and protect data in transit at rest.

### Reliability

Ability of a system to:
* Recover from infrastructure or service disruptions;
* Dynamically acquire computing resources to meet demand;
* Mitigate disruptions such as transient network issues or misconfigurations;
* Tsting recovery procedures;
* Scaling horizontally to increase aggregate system availability;
* Automatically recovering from failure.

### Performance Efficiency

Ability to use computing resources efficiently to meet system requirements and to maintain that efficiency as demand changes and technologies evolve.

Evaluating the performance efficiency of your architecture icnludes experimenting more often, using serverless architectures, and seigning systems to be able to go global in minutes.

## Cost Optimization

Ability to run systems to deliver business value at the lowest price.

It includes adopting a consumption model, analyzing and attributing expenditure and using managed services to reduce the cost of the ownership.

## Using this tool

Free tool to review the state of your workload.

First, identify the workload to review, then answer a series of questions about your architecture about the five pillars.

It then provides a plan for you to use the cloud best practices.
