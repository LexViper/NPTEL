# NPTEL Cloud Computing: Week 1 Cheat Sheet
Quick revision guide for Week 1 (Lectures 1–5) of NPTEL Cloud Computing, tailored for the 100-MCQ exam on May 3, 2025. Summarizes key points for computing, trends, distributed computing, cloud computing, service models, and networking.

## Computing
- **Definition**: Goal-oriented activity using computers (e.g., apps, data, science).
- **Trends**: Distributed → Grid → Cluster → Utility → Cloud.

## Trends in Computing
- **Distributed Computing**:
  - **What**: Autonomous computers, local memory, message-passing.
  - **Examples**: Internet, ATMs, intranets.
  - **Components**: Workstations, servers, personal devices.
  - **Properties** (FRESH): Fault Tolerance, Resource Sharing, Easy Expand, Scalability, High Performance.
  - **Why**: Large-scale apps, fault tolerance.
- **Grid Computing**:
  - **What**: Dispersed computers pool resources via middleware.
  - **Examples**: SETI@home, Folding@home, CERN LHC.
  - **Components**: Nodes, middleware, networks.
  - **Properties** (SHARE): Shared Resources, Heterogeneous, Accessible, Research-Focused, Expandable.
  - **Why**: Compute/data-intensive research.
- **Cluster Computing**:
  - **What**: Local, tightly coupled computers as one system.
  - **Examples**: Google search clusters, Pixar render farms.
  - **Components**: Nodes, high-speed network, master node.
  - **Properties** (FAST): Fast Processing, All-in-One, Scalable, Tight Coupling.
  - **Why**: High-performance computing.
- **Utility Computing**:
  - **What**: Rent resources, pay-per-use.
  - **Examples**: Early AWS, IBM on-demand.
  - **Components**: Resource pools, billing system, access portal.
  - **Properties** (RENT): Resource Access, Economical, No Ownership, Temporary.
  - **Why**: Cost-effective for variable loads.
- **Cloud Computing**:
  - **What**: Internet-based, virtualized, scalable resources.
  - **Examples**: Google Drive, Azure, Salesforce.
  - **Components**: Virtual machines, cloud servers, internet.
  - **Properties** (GROW): Global Access, Resilient, On-Demand, Wide Scaling.
  - **Why**: Flexible, scalable apps.

## Distributed Computing (Detailed)
- **What**: Many computers with own memory, talk via messages.
- **Examples**: Internet, ATMs, intranets.
- **Components**: Workstations (user PCs), servers (resources), personal devices (phones).
- **Properties** (FRESH):
  - **F**ault Tolerance: Survives failures.
  - **R**esource Sharing: Shared CPU/storage.
  - **E**asy Expand: Add nodes easily.
  - **S**calability: Handle more work.
  - **H**igh Performance: Faster together.
- **Why**: Compute-intensive (e.g., Pi), data-intensive (e.g., LHC), no SPOF.

## Cloud vs. Client-Server
- **Client-Server**: Simple, limited scaling, no virtualization.
- **Cloud**: Virtualized, load-balanced, scalable.
- **Analogy**: IaaS = roads, PaaS = cars, SaaS = passengers.

## Service Models (XaaS)
- **SaaS** (Software as a Service):
  - **What**: Web apps, no install (e.g., Gmail).
  - **Features**: Central management, no upgrades, one-to-many, APIs.
  - **Use Cases**: Email campaigns, mobile, short-term, spiky demand.
  - **Not For**: Real-time, regulated data, on-premise needs.
  - **Examples**: Salesforce (CRM, pay-per-use), Gmail (email, free).
- **PaaS** (Platform as a Service):
  - **What**: Coding platform (e.g., Azure).
  - **Features**: Multi-tenant, auto-scaling, team tools, web UI.
  - **Use Cases**: Team coding, agile dev, automation.
  - **Not For**: Portable apps, proprietary languages, custom hardware.
  - **Examples**: App Engine (Python/Java), Azure (.NET).
- **IaaS** (Infrastructure as a Service):
  - **What**: Rent servers/storage (e.g., EC2).
  - **Features**: Dynamic scaling, utility pricing, multi-user.
  - **Use Cases**: Volatile demand, startups, rapid growth, trials.
  - **Not For**: Regulated data, high-performance on-premise.
  - **Examples**: Amazon EC2 (hourly), Rackspace (hourly).

## Networking
- **Dynamic Provisioning**: Networks adjust fast.
- **Tools**: VLANs (split), VPNs (secure), OpenSSH/OpenVPN (setup).
- **OSI Layers**:
  - 7 layers: Physical → Application.
  - SaaS: Provider all.
  - PaaS: Consumer app, provider rest.
  - IaaS: Consumer app/transport, provider lower.
- **NFV**: Virtual network functions on standard servers, not special hardware.

## MCQ Tips
- Know definitions (distributed, grid, SaaS).
- Compare models (SaaS vs. PaaS, cloud vs. client-server).
- Memorize examples (Gmail = SaaS, EC2 = IaaS).
- Study tables (providers, OSI layers).
- Understand use cases/limitations (e.g., no IaaS for regulated data).