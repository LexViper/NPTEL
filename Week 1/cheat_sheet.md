# NPTEL Cloud Computing: Week 1 Cheat Sheet

Quick revision guide for **Week 1** (Lectures 1–5) of **NPTEL Cloud Computing**, tailored for the **100-MCQ exam** on **May 3, 2025**. Summarizes key points for computing, trends, distributed computing, cloud computing, service models, and networking in a **compact, MCQ-ready** format.

---

## Computing

- **Definition**:  
  Goal-oriented activity using computers (e.g., apps, data, science).  

- **Trends**:  
  Distributed → Grid → Cluster → Utility → Cloud  

---

## Trends in Computing

| **Trend**            | **What**                                          | **Examples**                          | **Components**                             | **Properties (Mnemonic)**                     | **Why**                              |
|-----------------------|--------------------------------------------------|---------------------------------------|--------------------------------------------|----------------------------------------------|--------------------------------------|
| **Distributed**       | Autonomous computers, local memory, message-passing | Internet, ATMs, intranets            | Workstations, servers, personal devices     | *FRESH*: Fault Tolerance, Resource Sharing, Easy Expand, Scalability, High Performance | Large-scale apps, fault tolerance    |
| **Grid**              | Dispersed computers pool resources via middleware | SETI@home, Folding@home, CERN LHC    | Nodes, middleware, networks                 | *SHARE*: Shared Resources, Heterogeneous, Accessible, Research-Focused, Expandable | Compute/data-intensive research      |
| **Cluster**           | Local, tightly coupled computers as one system    | Google search clusters, Pixar render farms | Nodes, high-speed network, master node     | *FAST*: Fast Processing, All-in-One, Scalable, Tight Coupling | High-performance computing           |
| **Utility**           | Rent resources, pay-per-use                       | Early AWS, IBM on-demand             | Resource pools, billing system, access portal | *RENT*: Resource Access, Economical, No Ownership, Temporary | Cost-effective for variable loads    |
| **Cloud**             | Internet-based, virtualized, scalable resources   | Google Drive, Azure, Salesforce       | Virtual machines, cloud servers, internet   | *GROW*: Global Access, Resilient, On-Demand, Wide Scaling | Flexible, scalable apps              |

---

## Distributed Computing (Detailed)

- **What**:  
  Many computers with own memory, talk via messages.  

- **Examples**:  
  - Internet  
  - ATMs  
  - Intranets  

- **Components**:  
  - **Workstations**: User PCs (e.g., laptops).  
  - **Servers**: Resources (e.g., databases).  
  - **Personal Devices**: Phones, tablets.  

- **Properties** (*FRESH*):  
  - **F**ault Tolerance: Survives failures.  
  - **R**esource Sharing: Shared CPU/storage.  
  - **E**asy Expand: Add nodes easily.  
  - **S**calability: Handle more work.  
  - **H**igh Performance: Faster together.  

- **Why**:  
  - Compute-intensive (e.g., Pi calculation).  
  - Data-intensive (e.g., LHC data).  
  - No single point of failure (SPOF).  

---

## Cloud vs. Client-Server

- **Client-Server**:  
  Simple, limited scaling, no virtualization.  

- **Cloud**:  
  Virtualized, load-balanced, scalable.  

- **Analogy**:  
  - IaaS = roads  
  - PaaS = cars  
  - SaaS = passengers  

---

## Service Models (XaaS)

| **Model** | **What**                     | **Features**                                  | **Use Cases**                          | **Not For**                              | **Examples**                     |
|-----------|------------------------------|-----------------------------------------------|----------------------------------------|------------------------------------------|----------------------------------|
| **SaaS**  | Web apps, no install         | Central management, no upgrades, one-to-many, APIs | Email campaigns, mobile, short-term, spiky demand | Real-time, regulated data, on-premise needs | Salesforce (CRM, pay-per-use), Gmail (free) |
| **PaaS**  | Coding platform              | Multi-tenant, auto-scaling, team tools, web UI | Team coding, agile dev, automation     | Portable apps, proprietary languages, custom hardware | App Engine (Python/Java), Azure (.NET) |
| **IaaS**  | Rent servers/storage         | Dynamic scaling, utility pricing, multi-user  | Volatile demand, startups, rapid growth, trials | Regulated data, high-performance on-premise | Amazon EC2 (hourly), Rackspace (hourly) |

---

## Networking

- **Dynamic Provisioning**:  
  Networks adjust fast.  

- **Tools**:  
  - **VLANs**: Split networks.  
  - **VPNs**: Secure links.  
  - **OpenSSH/OpenVPN**: Setup tools.  

- **OSI Layers**:  
  - **7 Layers**: Physical, Data Link, Network, Transport, Session, Presentation, Application.  
  - **SaaS**: Provider handles all.  
  - **PaaS**: Consumer app layer, provider rest.  
  - **IaaS**: Consumer app/transport, provider lower.  

- **NFV**:  
  Virtual network functions on standard servers, not special hardware.  

---

## MCQ Tips

- **Know Definitions**: Distributed, grid, SaaS.  
- **Compare Models**: SaaS vs. PaaS, cloud vs. client-server.  
- **Memorize Examples**: Gmail = SaaS, EC2 = IaaS.  
- **Study Tables**: Providers, OSI layers.  
- **Understand Use Cases/Limitations**: e.g., no IaaS for regulated data.  

---

*End of Week 1 Cheat Sheet*
