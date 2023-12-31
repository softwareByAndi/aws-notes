<link rel="stylesheet" href="./css/globals.css">

# Resources & Links

## Compute Links
- [compute resource list](https://aws.amazon.com/products/compute/)
- [compute blog](https://aws.amazon.com/blogs/compute/)
- [compute services](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/compute-services.html)
- [hands-on compute tutorials](https://aws.amazon.com/getting-started/hands-on/?awsf.getting-started-category=category%23compute&awsf.getting-started-content-type=content-type%23hands-on&getting-started-all.sort-by=item.additionalFields.content-latest-publish-date&getting-started-all.sort-order=desc)
- [category deep dive: serverless](https://aws.amazon.com/getting-started/hands-on/?awsf.getting-started-category=category%23compute&awsf.getting-started-content-type=content-type%23hands-on&getting-started-all.sort-by=item.additionalFields.content-latest-publish-date&getting-started-all.sort-order=desc)




# Notes: Compute Services

## Server Computing Options

### EC2 ( Elastic Compute )
a server host
- host traditional applications
- provides full access to the OS
- need to provision & manages servers


## Serverless Computing Options
- provision instances (virtual servers)
- upload your code
- continue to manage the instances while your application is running

### AWS Lambda
designed for quick processes that run in <em>under 15 minutes</em>
- upload code into lambda function
- configure trigger
- spins up a auto scaling environment on demand to run function

when to use:
- no provisioning or manage servers
- host short running functions
- service-oriented applications
- event driven applications


### AWS Fargate
a serverless compute engine <em>for containers</em> ( ECS &/or EKS )
- manages server infrastructure for you
    - i.e. do not need to provision or manage servers 
- pay only for resources required to run the containers
- for situations where you don't want or need to use an EC2 host


---

## Container Orchestration Tools
containers package up code, dependencies and configurations
- is a docker container
- run on top of EC2 or Fargate instances
- run in isolation from other containers / instances


### Amazon Elastic Container Service (ECS)

### Amazon Elastic Kubernetes Service (EKS)

---




# Notes: EC2 (Elastic Compute)

## Instance Types
- [# General Purpose](#general-purpose-instance)
- [# Compute Optimized](#compute-optimized-instance)
- [# Memory Optimized](#memory-optimized-instance)
- [# Storage Optimized](#storage-optimized-instance)
- [# Accelerated Computing](#accelerated-computing-instance)


### General Purpose Instance
ideal for balanced resources
- diverse workloads
- web servers
- code repositories
- small & medium databases


### Compute Optimized Instance
ideal for compute intensive tasks
- gaming servers
- high performance computing (HPC)
- scientific modeling
- batch processing workloads that require processing many transactions in a single group


### Memory Optimized Instance
ideal for memory intensive tasks
- high performance databases
- workloads that process large datasets in memory
- workloads that require large amounts of data to be preloaded before running an application


### Storage Optimized Instance
ideal for workload that require high perfomrance for locally stored data
- distributed file systems
- data warehousing applications
- high-frequency online transaction prcessing (OLTP) systems

### Accelerated Computing Instance
ideal for tasks that utilize hardware accelerators or coprocessors
- floating point number calculations
- graphics processing
- data pattern matching
- game streaming
- application streaming

---

## Pricing Options

- [On Demand](#on-demand-pricing)
- [Savings Plans](#savings-plans-pricing)
- [Reserved Instances](#reserved-instances-pricing)
- [Spot Instances](#spot-instances-pricing)
- [Dedicated Hosts](#dedicated-hosts-pricing)


### On Demand Pricing
ideas for short-term, irregular workloads that <em>cannot be interrupted</em> 
- no upfront costs
- no minimum contracts
- instances run until stopped
- only pay for the compute time used

examples:
- developing and testing applications
- running applicatios that have unpredictable usage patterns

not recommended for workloads that last a year or longer ( <em>use reserved instances instead</em> )

### Savings Plans Pricing
for long-term, steady apps that have a predictable amount of traffic
- cost savings up to -72% ( compared to on-demand costs ) 
- 1-3 year contract
- commit to a consistent amount of compute usage for the contract term
- usage above committed amount is charged on-demand rates

see AWS Cost Explorer to visualize and analyze cost & usage over time

### Reserved Instances Pricing
a billing discount applied to the use of on demand instances
- 1 or 3 year term

options include:
- Standard Reserved
- Convertable Reserved
- Scheduled Reserved

### Spot Instances Pricing
ideal for workloads w/ flexible start and end times that <em>can withstand interruptions</em>
- use unused computing capacity
- cost savings up to -90% ( compared to on-demand costs )


### Dedicated Hosts Pricing
fully dedicated physical servers
- most expensive
- meet legal requirements for certain applications