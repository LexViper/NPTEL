# Week 11 Cloud Computing Cheatsheet 🚀

## Lecture 51: Dew Computing 🌧️

### Overview 📝
- **Definition**: Combines cloud computing with end-device capabilities (PCs, phones) to enhance user experience, reducing internet dependency.
- **Goal**: Enable offline data access, rapid creation/editing with minimal network management.

### Features 🌟
- **Independence**: Local device operates without constant internet.
- **Collaboration**: Syncs with cloud when connected.
- **Analogy**: Cloud (remote), Fog (near), Dew (on-device).

### Architecture 🏗️
- **Dew Virtual Machine (DVM)**: Isolated environment for dew server.
- **Dew Server Functions**: Serve users, sync local/remote data, achieve data replication, distribution, synchronization.

### Applications 📱
- **Web in Dew (WiD)**: Local WWW fraction, syncs with web.
- **Storage in Dew (SiD)**: Local storage synced to cloud (e.g., Dropbox).
- **Database in Dew (DBiD)**: Dual databases, one as backup.
- **Software in Dew (SiD)**: Cloud-saved software configs (e.g., App Store).
- **Platform in Dew (PiD)**: Local dev suite, cloud-synced (e.g., GitHub).
- **Infrastructure as Dew (IaD)**: Cloud-backed local device.

### Challenges ⚠️
- Power management, processor utility, data storage, OS viability, programming, database security.

## Lectures 52 & 53: Serverless Computing - I & II ⚙️

### Overview 📦
- **Definition**: Cloud model for running backend services on-demand, no infrastructure management.
- **Focus**: Developers write code (functions), providers handle scaling, provisioning.

### Types 🌐
- **Backend-as-a-Service (BaaS)**: Off-the-shelf services (e.g., Firebase for databases).
- **Function-as-a-Service (FaaS)**: Event-driven, stateless functions (e.g., AWS Lambda).

### Major Providers 🏢
- **AWS Lambda**: Event-driven, executes code in response to AWS events (e.g., S3 changes).
- **Google Cloud Functions**: Triggered by GCP events (e.g., Cloud Storage uploads).
- **Azure Functions**: Flexible language support, consumption-based pricing.

### Challenges 🚧
- Asynchronous calls, function interdependencies, shared code issues, library overload, tech diversity, excessive functions.

## Lectures 54 & 55: Sustainable Cloud Computing - I & II 🌍

### Overview 🌱
- **Goal**: Minimize energy use, carbon footprints, ensure reliability in Cloud Data Centers (CDCs).
- **Energy Consumption**: CDCs projected to use 8000 TWh by 2030.

### Components 🛠️
- **Application Model**: Data/function parallel, message passing for energy efficiency.
- **Thermal-aware Scheduling**: Manages heat via single/multi-core, reactive/proactive methods.
- **Virtualization**: VM migration for load balancing, renewable energy use.
- **Capacity Planning**: Optimize power, IT, workloads for ROI.
- **Renewable Energy**: Solar/wind to reduce carbon emissions.
- **Waste Heat Utilization**: Vapor-absorption cooling to reuse heat.

### Taxonomy 📊
- Application design, sustainability metrics, capacity planning, energy management, virtualization, thermal scheduling, cooling, renewable energy, waste heat utilization.

### Challenges ⚖️
- Balancing energy efficiency with reliability, avoiding SLA violations, managing renewable energy unpredictability.

### References 📚
- Wang, Y., *Dew Computing*, 2016.
- Buyya, R., Gill, S., *Sustainable Cloud Computing*, 2018.
- AWS Lambda, Google Cloud Functions, Azure Functions documentation.