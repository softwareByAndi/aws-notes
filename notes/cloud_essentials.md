<style>
    :root {
        background-color: #0B0B0A;

        --color-dark-red: #982649;
        --color-light-red: #D75B80;
        --color-purple: #9489D1;
        --color-dark-gray: #7C8483;
        --color-light-gray: #CFCFC9;
        --color-blue-gray: #71A2B6;
        --color-highlight: #EDB88B;
        --color-light-blue: #97BCD8;
    }

    em { color: var(--color-highlight); font-style: normal; }

    p { color:var(--color-light-gray); }
    li { color:var(--color-dark-gray); }
    a { color:var(--color-purple); text-decoration: underline; }
    a:hover { 
        font-weight:900; 
        color:var(--color-purple); 
        text-decoration: underline; 
    }

    h1 { color:var(--color-light-gray); }
    h2 { font-weight:700; margin-top:2rem; color:var(--color-light-gray); }
    h3 { font-weight:700; margin-top:2rem; color:var(--color-light-blue); }
    h4 { font-weight:800; margin-top:2rem; color:var(--color-dark-red); }

</style>

# EC2 (Elastic Compute)

## Instance Types
- [General Purpose](#general-purpose-instance)
- [Compute Optimized](#compute-optimized-instance)
- [Memory Optimized](#memory-optimized-instance)
- [Storage Optimized](#storage-optimized-instance)
- [Accelerated Computing](#accelerated-computing-instance)


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


