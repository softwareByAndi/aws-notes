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

    highlight { color: var(--color-highlight); }

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
