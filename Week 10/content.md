# Week 10: Cloud Computing Paradigm 📚

## Lectures 45 & 46: Cloud Migration - I & II 🌐

### Concepts Covered 🚀
- **VM Migration Basics**: Move running apps/VMs between servers, including CPU state, storage, memory, network 🖥️.
- **Migration Strategies**: Cold (Non-Live) and Hot (Live), with Pre-copy and Post-copy for live migration 🔄.
- **Needs for VM Migration**:
  - **Load Balancing**: Fair workload distribution ⚖️.
  - **Maintenance**: Transparent migration during upkeep 🔧.
  - **Operational Efficiency**: Consolidate VMs to save power 💡.
  - **Quality-of-Service (QoS)**: Switch providers if QoS unmet 📉.
  - **Fault Tolerance**: Relocate VMs during failures 🛡️.
- **When to Migrate?** ⏰
  - Decommission machines, relieve congested hosts.
- **Migration Costs**: Communication overhead, migration time, downtime 📊.
- **Concerns**:
  - Minimize downtime (service unavailability) ⏱️.
  - Reduce migration time ⏲️.
  - Avoid resource contention (CPU, network) 🚫.

### VM Migration Types 🛠️
- **Cold (Non-Live)**: VM off/suspended, high downtime 😴.
- **Hot (Live)**: VM runs, suitable for real-time apps 🚀.

### Live VM Migration 🔍
- **Components**:
  - CPU context, memory 📝.
  - Disk (less critical with NAS/mirrored disks) 💾.
  - Network (IP/MAC with minimal packet loss) 🌐.
  - I/O devices (virtual I/O simpler) 🖱️.
- **Memory Migration**:
  - **Push**: Pages sent while VM runs, re-send modified 📤.
  - **Stop-and-Copy**: Stop VM, copy pages, restart 📥.
  - **Pull**: Destination pulls pages as needed 📲.
- **Pure Stop-and-Copy**: Simple, but downtime scales with memory size, not for live services 🚫.

### Live Migration Phases 🔄
- **Pre-Copy Approach**:
  - **Pre-Copy Phase**: VM runs, memory copied iteratively, dirty pages re-sent 📜.
  - **Termination Phase**: Stops when:
    - Rounds exceed threshold 🔢.
    - Transmitted memory exceeds limit 📏.
    - Dirty pages below threshold 📉.
  - **Stop-and-Copy Phase**: Suspend VM, copy dirty pages/CPU state, resume at destination 🔄.
  - **Restart Phase**: VM restarts on destination 🖥️.
  - Used by KVM, Xen, VMware 🛠️.
- **Post-Copy Approach**:
  - **Stop Phase**: Stop VM, copy CPU state 📝.
  - **Restart Phase**: Start VM at destination 🚀.
  - **On-Demand Copy**: Copy memory as needed, uses demand paging/pre-paging 📜.

### Migration Analysis 📊
- **Non-Live**:
  - Migration time: \( T_{mig} = \frac{V_m}{R} \), (\( V_m \): VM memory, \( R \): rate) ⏲️.
  - Downtime: \( T_{down} = T_{mig} \) ⏱️.
- **Pre-Copy**:
  - Migration: \( T_{i,mig} = \frac{V_m}{R} \left( \frac{1 - r^{n+1}}{1 - r} \right) + T_{res} \).
  - Downtime: \( T_{i,down} = r^n \left( \frac{V_m}{R} \right) + T_{res} \).
  - \( r = \frac{P \cdot D}{R} \), \( P \): page size, \( D \): dirtying rate, \( T_{res} \): restart ⏲️.
  - Rounds: \( n = \min \left( \left\lceil \log_r \frac{V_{th}}{V_m} \right\rceil, n_{max} \right) \).
- **Multiple VMs**:
  - **Serial**:
    - First VM pre-copies, others suspended during stop-and-copy.
    - Downtime: \( T_{down} = \frac{V_m}{R} \cdot r^n + (m-1) \frac{V_m}{R} \left( \frac{1 + r^{n+1}}{1 - r} \right) + T_{res} \).
  - **Parallel**:
    - All VMs pre-copy, share \( R/m \).
    - Migration: \( T_{mig} = \frac{m \cdot V_m}{R} \cdot \left( \frac{1 - (mr)^{n(p)+1}}{1 - mr} \right) + T_{res} \).
    - Downtime: \( T_{down} = \frac{m \cdot V_m}{R} \cdot (m \cdot r)^{n(p)} + T_{res} \).

### References 📚
- Kai Hwang, *Distributed and Cloud Computing*, 2012.
- Clark, C., *Live Migration of Virtual Machines*, NSDI, 2005.
- Hines, M., *Post-Copy Based Live Virtual Machine Migration*, 2009.
- Choudhary, A., *A Critical Survey of Live Virtual Machine Techniques*, 2017.

## Lectures 47 & 48: Container-based Virtualization - I & II (Docker) 🐳

### Concepts Covered 🚀
- **Containers**: Lightweight virtualization, packages code + dependencies 📦.
- **Container-based Virtualization**: OS-level, shares host kernel, unlike VM hardware virtualization 🖥️.
- **Kubernetes**: Automates deployment, scaling, management of containers 🌐.
- **Docker**: Standard, lightweight, secure platform for apps 🛳️.

### Containers Introduction 📝
- **Definition**: Packages code + dependencies (runtimes, libraries) for consistent execution 🌍.
- **Docker**: Develop, ship, run apps in containers 🐳.
- **Kubernetes**: Manages workloads, offers deployment, scaling, load balancing 🛠️.

### Containers Needs and Benefits 🎉
- **Needs**:
  - **Abstraction**: Decouples apps from environment 🔄.
  - **Agile Development**: Simplifies dependency management 🚀.
  - **Efficiency**: Minimal resources 💡.
  - **Portability**: Runs on Linux, Windows, Mac, cloud 🌐.
- **Benefits**:
  - **Separation**: Developers on logic, operations on deployment 👥.
  - **Portability**: Consistent across environments 🌍.
  - **Isolation**: Virtualizes CPU, memory, storage, network 🔒.

### Containers vs. VMs ⚖️
- **VMs**: Full guest OS, hardware virtualization, resource-heavy 🖥️.
- **Containers**: Share host OS, lightweight, memory-efficient 🚀.
- **Comparison**:
  - Containers: Less memory, faster startup ⏩.
  - Similar isolation, relaxed properties 🔒.

### Kubernetes Components 🛠️
- **Cluster**: Worker nodes run Pods (apps) 📥.
- **Control Plane**: Manages nodes/Pods, fault-tolerant 🔄.

### Docker Engine 🐳
- **Features**:
  - **Standard**: Industry-standard containers 📦.
  - **Lightweight**: Shares OS kernel, low costs 💡.
  - **Secure**: Strong isolation 🔒.
- **Container Image**: Standalone package with code, runtime, tools, libraries 📦.

### Docker Overview 📜
- **Purpose**: Simplifies deployment with portable units 🚚.
- **Advantages**:
  - Unified pipeline, less maintenance 🛠️.
  - Preserves software stacks 📚.
  - Transparent build for debugging 🔍.

### References 📚
- https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/
- https://www.docker.com/resources/what-container
- https://cloud.google.com/learn/what-are-containers
- *Docker in Practice*, Ian Miell and Aidan Hobson Sayers, 2019.

## Lectures 49 & 50: Docker Container - Demo (Part-I & II) 🖱️

### Concepts Covered 🚀
- **Docker Demo**: Run MySQL and PHPMyAdmin on Docker 🗄️.

### Demo Objective 🎯
- **Setup**: Deploy MySQL (database) and PHPMyAdmin (GUI) using Docker 🐳.
- **Purpose**: Show container benefits over standalone systems 📦.

### Standalone System (No Container) 🚫
- **Requirements**:
  - Install MySQL, Apache, PHP, PHPMyAdmin separately 🛠️.
- **Migration Challenges**:
  - Reinstall components on new machine 🔧.
  - Manual backup/restore of MySQL data 📜.

### Containers Benefits 🎉
- **Separation**: Developers on logic, operations on deployment 👥.
- **Portability**: Runs anywhere (Linux, Windows, cloud) 🌍.
- **Isolation**: OS-level resource isolation 🔒.

### Deployment Comparison 🏗️
- **Traditional**: Physical servers, no resource boundaries 🚫.
- **Virtualized**: VMs with full OS, heavy 🖥️.
- **Container**: Shares OS, lightweight, portable 📦.

### References 📚
- https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/
- https://www.docker.com/resources/what-container
- https://cloud.google.com/learn/what-are-containers