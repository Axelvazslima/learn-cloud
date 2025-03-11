# Elastic Compute Cloud (EC2) Types And Families

Each EC2 instance type is grouped under an instance family and are optimized for certain types of tasks.

Combination of CPU, memory, storage and networking capacity.

## Families

### General purpose

Good balance of compute memory and networking resources -> balanced resources.

Diverse workloads, like web servers or code repositories.

```sh
Application gaming and backend servers. Small and medium databases.
```

Application with similar needs in all areas -> no need for specific optimization.

> Balanced resources.

### Compute optimized

Intensive tasks, gaming servers, high performance computing (HPC) and scientific modeling.

```sh
Web, applications and gaming servers -> Dedicated servers.
```

> High performance processors.

### Memory optimized

Memory intensive tasks.

Fast performance for processing large datasets in memory.

Memory is a temporary storage area that holds all the data and instruction the CPU needs to be able to complete actions. Before a program runs, it needs to be loaded from storage into memory -> CPU get direct access to the computer program.

```sh
Large amount of data needs to be preloaded before running an application.
```

> High performance database and real-time processing of unstructured data.

### Accelerated computing

Floating-point number calculations, graphic processing, data pattern matching and utilize hardware accelerators or coprocessors.

Perform some functions more efficiently than is possible in software running on CPUs.

A hardware accelerator is a component that can expedite data processing -> Ideal for workloads.

```sh
Graphic application, game streaming and application streaming.
```

> Hardware accelerator and coprocessors.

### Storage optimized

High performance for locally stored data.

High sequential read and write access to large datasets on local storage.

```sh
Distributed files systems, data warehouse applications and high-frequency online transaction processing (OLTP) systems.
```

Ideal for great input/output. I/O has a metric to measure speed [performance]: Input/output operations per second (IOPS).

Designed to deliver tens of thousands of low-latency, random IOPS to applications.

> High Input/Output per second requirement.
