# Week 10 Cloud Computing Cheatsheet 🚀

## Lectures 45 & 46: Cloud Migration - I & II 🌐

### VM Migration Overview 🖥️
- **Definition**: Move VMs/apps between hosts, including CPU, memory, storage, network.
- **Why Migrate?** 🔄
  - Load balancing, maintenance, power efficiency, QoS, fault tolerance.
- **When?** ⏰
  - Decommission machines, reduce load on congested hosts.
- **Costs**: Overhead, migration time, downtime.
- **Concerns**: Minimize downtime, migration time, resource contention.

### Migration Types 🛠️
- **Cold (Non-Live)**: VM off/suspended, high downtime 😴.
- **Hot (Live)**: VM runs during migration, ideal for real-time apps 🚀.

### Live Migration 🔍
- **Components**: CPU, memory, disk (if not NAS), network (IP/MAC), I/O devices.
- **Memory Migration**:
  - **Push**: Send pages while VM runs, re-send modified pages 📤.
  - **Stop-and-Copy**: Stop VM, copy pages, restart 📥.
  - **Pull**: Destination pulls pages as needed 📲.
- **Pre-Copy**:
  - Iterative memory copy, stop when thresholds met (rounds, memory, dirty pages).
  - Stop-and-copy for remaining data, restart.
  - Used by KVM, Xen, VMware 🛠️.
- **Post-Copy**:
  - Copy CPU state, start VM, copy memory on-demand.
  - Uses demand paging, pre-paging 📜.

### Migration Analysis 📊
- **Non-Live**: \( T_{mig} = T_{down} = \frac{V_m}{R} \) (\( V_m \): VM memory, \( R \): rate).
- **Pre-Copy**:
  - Migration: \( T_{mig} = \frac{V_m}{R} \left( \frac{1 - r^{n+1}}{1 - r} \right) + T_{res} \).
  - Downtime: \( T_{down} = r^n \left( \frac{V_m}{R} \right) + T_{res} \).
  - \( r = \frac{P \cdot D}{R} \), \( P \): page size, \( D \): dirtying rate, \( T_{res} \): restart.
  - Rounds: \( n = \min \left( \left\lceil \log_r \frac{V_{th}}{V_m} \right\rceil, n_{max} \right) \).
- **Multiple VMs**:
  - **Serial**: First VM pre-copies, others suspended.
  - **Parallel**: All pre-copy, share \( R/m \).

## Lectures 47 & 48: Container-based Virtualization - I & II (Docker) 🐳

### Containers 📦
- **Definition**: Lightweight virtualization, packages code + dependencies.
- **Docker**: Build, ship, run containerized apps 🛳️.
- **Kubernetes**: Automates deployment, scaling, management 🌐.

### Containers vs. VMs ⚖️
- **VMs**: Full guest OS, hardware virtualization, heavy 🖥️.
- **Containers**: Share host OS, lightweight, fast 🚀.

### Benefits 🎉
- **Portability**: Runs anywhere (Linux, Windows, cloud) 🌍.
- **Isolation**: Virtualizes CPU, memory, storage, network 🔒.
- **Efficiency**: Minimal resources 💡.
- **Separation**: Developers on logic, operations on deployment 👥.

### Kubernetes 🛠️
- **Cluster**: Worker nodes run Pods (apps) 📥.
- **Control Plane**: Manages nodes/Pods, fault-tolerant 🔄.

### Docker Engine 🐳
- **Features**: Standard, lightweight, secure 🔒.
- **Container Image**: Code, runtime, libraries, settings 📦.

## Lectures 49 & 50: Docker Container - Demo (Part-I & II) 🖱️

### Demo: MySQL + PHPMyAdmin 🗄️
- **Objective**: Run MySQL (database) and PHPMyAdmin (GUI) on Docker.
- **Standalone Issues**:
  - Separate installs for MySQL, Apache, PHP, PHPMyAdmin 🛠️.
  - Migration needs reinstall, manual backup 📜.
- **Container Benefits**:
  - Simplified deployment, portability, isolation 🚀.

### Deployment Types 🏗️
- **Traditional**: Physical servers, no boundaries 🚫.
- **Virtualized**: VMs with full OS, heavy 🖥️.
- **Container**: Shares OS, lightweight, portable 📦.

### References 📚
- Hwang, K., *Distributed and Cloud Computing*, 2012.
- Clark, C., *Live Migration of Virtual Machines*, 2005.
- https://kubernetes.io/, https://www.docker.com/, https://cloud.google.com/learn/what-are-containers