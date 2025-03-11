# Scaling in Amazon Elastic Cloud Computing (EC2)

Prevents idle resources or not having them.

```sh
"Everything fails all the time, so plan for failure and nothiung fails."
```

Begging with only the resources you need and designing your architecture to automatically respond to changing demand by scaling out or in.

The AWS service that provides this EC2 auto scaling for you to not need to worry about paying too much or not having the needed resources is **Amazon EC2 Auto Scaling**.

## Amazon EC2 Auto Scaling

Problem: Website that wouldn't load and frequently timed out -> the site might have received more requests than it was able to handle.

This AWS service enables you to automatically add or remove Amazon EC2 instances in response to changing application demand -> maintain a great sense of *application availability*.

> Dynamic Scaling: Responds to chaning demand.

> Predictive Scaling: Automatically schedules the right number of Amazon EC2 instances based on predicted demand.

To scale faster, you can use dynamic scaling and predictive scaling together.

### Scaling up

Adding more power to the machines that are running.

### Scaling out

More machines to work together.

In the cloud, *power is a programmatic resource*, so you can take a more flexible approach to the issue of scaling.

By adding EC2 Auto Scaling to an app, you can add new instances when necessary and terminate them when you no longer need it.

### Auto Scaling Group

sum(Minimun X Desired X Scale as needed) = maximum

> The minimun capacity is the number of Amazon EC2 instances that launches immediately after you have created the Auto Scaling group.

> The desired capacity is the most optimal amount of EC2 instances in your app. If you specify it, the default is the *minimun*.

> The maximum capacity is the most amount of EC2 instances you can add to your app.

Amazon EC2 Auto Scaling uses Amazon EC2 instances, meaning you only **pay for what you use** -> cost-effective architecture that provides the best experience to the customers while reducing expenses.
