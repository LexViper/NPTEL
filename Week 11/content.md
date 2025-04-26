# Week 11: Cloud Computing Paradigms 📚

## Lecture 51: Dew Computing 🌧️

### Concepts Covered 🚀
- **Dew Computing Overview**: Combines cloud computing with end-device capabilities.
- **Features**: Independence and collaboration.
- **Architecture**: Dew Virtual Machine (DVM) and Dew Server.
- **Applications**: Web, storage, database, software, platform, infrastructure.
- **Challenges**: Resource management and security.

### Dew Computing (DC) 📝
- **Definition**: Enhances user experience by leveraging end devices (PCs, smartphones) alongside cloud computing, reducing internet reliance.
- **Characteristics**:
  - Micro-service-based, vertically distributed hierarchy.
  - Smart devices (phones, watches) process IoT data at network edge.
  - Operates offline, syncs with cloud when connected.
- **Goal**: Provide ubiquitous, user-centric services with minimal internet dependency.
- **Example**: Dropbox enables offline file access, syncs when online.

### Features 🌟
- **Independence**: Local device functions without constant internet.
- **Collaboration**: Syncs data with cloud services when connected.
- **Analogy**: Cloud (remote), Fog (near), Dew (on-device, like dew on ground).

### Architecture 🏗️
- **Dew Virtual Machine (DVM)**: Isolated environment for running dew server locally.
- **Dew Server Functions**:
  - Serve user requests.
  - Synchronize and correlate local/remote data.
  - Achieve data replication, distribution, synchronization.

### Applications 📱
- **Web in Dew (WiD)**: Local WWW fraction, syncs with web.
- **Storage in Dew (SiD)**: Local storage copied to cloud (e.g., Dropbox, Google Drive).
- **Database in Dew (DBiD)**: Dual databases, one as backup.
- **Software in Dew (SiD)**: Cloud-saved software configs (e.g., App Store, Google Play).
- **Platform in Dew (PiD)**: Local dev suite, cloud-synced (e.g., GitHub).
- **Infrastructure as Dew (IaD)**: Cloud-backed local device with DVM or settings sync.

### Challenges ⚠️
- Power management, processor utility, data storage, OS viability, programming principles, database security.

### References 📚
- Wang, Y., *Definition and Categorization of Dew Computing*, 2016.
- Ray, P.P., *An Introduction to Dew Computing*, IEEE Access, 2018.
- https://www.dropbox.com

## Lectures 52 & 53: Serverless Computing - I & II ⚙️

### Concepts Covered 🚀
- **Serverless Computing**: Backend services on-demand, no infrastructure management.
- **Function-as-a-Service (FaaS)**: Event-driven function execution.
- **Providers**: AWS Lambda, Google Cloud Functions, Azure Functions.

### Serverless Computing 📦
- **Definition**: Cloud model where developers deploy code without managing infrastructure; providers handle scaling, provisioning.
- **Characteristics**:
  - Event-driven, executed in stateless, ephemeral containers.
  - Developers focus on business logic, not system administration.
  - Pay-per-use billing for resources consumed.
- **Types**:
  - **Backend-as-a-Service (BaaS)**: Off-the-shelf services (e.g., Firebase for databases).
  - **Function-as-a-Service (FaaS)**: Stateless functions triggered by events (e.g., ExCamera for video processing).

### Challenges 🚧
- **Asynchronous Calls**: Increase system complexity.
- **Function Dependencies**: Debugging issues, extra costs for synchronous calls.
- **Shared Code**: Risks breaking functions, hitting size limits (e.g., 50MB in AWS Lambda).
- **Library Overload**: Increases warmup time, size limits.
- **Tech Diversity**: Adds maintenance complexity.
- **Excessive Functions**: Reduces maintainability, system understandability.

### Major Providers 🏢
- **AWS Lambda**:
  - Event-driven platform, executes code for AWS events (e.g., S3 bucket changes).
  - Supports Java, Python, Go, C#.
  - Charges only for execution time.
- **Google Cloud Functions**:
  - Triggered by GCP events (e.g., Cloud Storage uploads).
  - Fully managed, stateless, event-driven.
  - Supports HTTP, Pub/Sub, Firebase events.
- **Azure Functions**:
  - Supports C#, Java, JavaScript, Python, PowerShell.
  - Consumption plan for pay-per-use, Premium/App Service plans for specialized needs.
  - Common uses: APIs, IoT, big data, automation.

### References 📚
- Hong, S., *Go Serverless*, USENIX HotCloud, 2018.
- Schleier-Smith, J., *What Serverless Computing Is*, CACM, 2021.
- AWS Lambda, Google Cloud Functions, Azure Functions documentation.

## Lectures 54 & 55: Sustainable Cloud Computing - I & II 🌍

### Concepts Covered 🚀
- **Sustainable Computing**: Energy-efficient, eco-friendly cloud services.
- **Sustainable Cloud Computing**: Minimize energy, carbon footprints, ensure CDC reliability.

### Sustainable Cloud Computing 🌱
- **Goal**: Reduce energy consumption, carbon emissions, maintain reliability in Cloud Data Centers (CDCs).
- **Energy Consumption**: Projected to reach 8000 TWh by 2030.
- **Strategies**:
  - Use renewable energy (solar, wind).
  - Optimize resource management (servers, storage, cooling).
  - Relocate CDCs for waste heat recovery, green resources, free cooling.

### Components 🛠️
- **Application Model**: Data/function parallel, message passing for energy efficiency.
- **Thermal-aware Scheduling**: Single/multi-core, reactive/proactive to reduce hotspots, cooling needs.
- **Virtualization**: VM migration for load balancing, renewable energy utilization.
- **Capacity Planning**: Optimize power, IT, workloads for ROI.
- **Renewable Energy**: Solar/wind to reduce Carbon Usage Efficiency (CUE).
- **Waste Heat Utilization**: Vapor-absorption cooling to reuse heat, reduce cooling costs.

### Taxonomy 📊
- Application design, sustainability metrics, capacity planning, energy management, virtualization, thermal scheduling, cooling, renewable energy, waste heat utilization.

### Challenges ⚖️
- Balancing energy efficiency with reliability.
- Avoiding SLA violations due to resource switching (e.g., DVFS).
- Managing renewable energy unpredictability, high capital costs.

### References 📚
- Buyya, R., Gill, S., *Sustainable Cloud Computing*, 2018.
- Andrae, A.S.G., *On Global Electricity Usage*, 2015.
- Gill, S., Buyya, R., *A Taxonomy for Sustainable Cloud Computing*, ACM Comput. Surv., 2018.