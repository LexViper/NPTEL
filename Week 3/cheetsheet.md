
### 📜 Week 3: SLA & OpenStack Cheatsheet

#### 📘 1. Service Level Agreement (SLA) 🤝

**Definition:**  
A **contract** between a Service Provider (SP) and Service Consumer (SC) ensuring **service quality**, enforced via **Service Level Objectives (SLOs)** (e.g., 99.9% uptime). 🛠️

**Purpose:**  
Builds **trust** through measurable performance. 💪

**Key Components:**
- 📋 Services, definitions, responsibilities  
- 📈 Metrics (uptime, latency), auditing  
- 🔁 Remedies, review, and evolution

**Types of SLA:**
- 🏪 **Off-the-Shelf:** Fixed, standard terms (e.g., AWS)  
- 🏢 **Negotiable:** Tailored to enterprise requirements

**Web Service SLA Standards:**
- 💬 **WS-Agreement:** XML-based negotiation format  
- 📊 **WSLA:** XML-based QoS monitoring (e.g., response time)

---

#### 🔍 Cloud vs. Web SLA

| Aspect     | Cloud SLA ☁️            | Web SLA 🌐             |
|------------|--------------------------|------------------------|
| **QoS**     | Security, privacy         | Response time, cost    |
| **Automation** | High                     | Low                    |
| **Allocation** | Global, no UDDI          | UDDI-based             |

🧠 **Mnemonic:** SLA = **Services, Levels, Agreements**  
🎯 **Exam Tip:**  
- SLA = Contract  
- SLO = Measurable goal  

---

#### ⚙️ 2. OpenStack Components

| Component | Role         | Managed By | Analogy             |
|-----------|--------------|------------|---------------------|
| **Nova**    | Compute, VMs | Hypervisors | 👨‍🍳 Chef              |
| **Neutron** | Networking   | IPs, VLANs  | 🚦 Traffic cop         |
| **Cinder**  | Block storage| Persistent  | 🔌 USB drive           |
| **Swift**   | Object storage| Files/images | ☁️ Cloud Dropbox   |
| **Glance**  | Image service| Metadata    | 📚 Library catalog     |
| **Keystone**| Identity     | Auth/tokens | 🕴️ Bouncer             |
| **Horizon** | Dashboard    | Web UI      | 🚀 Spaceship panel     |

🧠 **Mnemonic:** NNCSGKH  
❓ **Exam Tip:** Focus on Nova Scheduler, Keystone tokens  

---

#### 💾 3. OpenStack Storage Types

| Type       | Persists        | Managed By | Use Case         | Analogy         |
|------------|------------------|------------|------------------|------------------|
| **Ephemeral** | Until VM ends   | Nova       | OS, scratch       | 💾 RAM           |
| **Block**     | Until deleted   | Cinder     | OS, disks         | 🖴 External drive |
| **Object**    | Until deleted   | Swift      | Images, backups   | ☁️ Google Drive   |

🎯 **Exam Tip:**  
- Ephemeral = Temporary  
- Block = Persistent disks  
- Object = Persistent files  

---

#### 🔄 4. VM Creation Workflow

1. 🖱️ **Horizon:** User login  
2. 🔐 **Keystone:** Token issued  
3. ⚙️ **Nova:** VM request, DB entry  
4. 🧠 **Scheduler:** Chooses compute node  
5. 🌐 **Neutron:** Network configuration  
6. 💾 **Cinder:** Block storage attached  
7. 🖼️ **Glance:** Retrieves image URI  
8. 📂 **Swift:** Supplies image  
9. 🚀 **Hypervisor:** Boots VM  

🧠 **Mnemonic:** **HKNSNGSH**  
❓ **Exam Tip:** Know the VM lifecycle sequence  

---

#### 🎯 5. Quick Exam Tips

- **SLAs:** Know parts, Cloud vs. Web, SLO vs. SLA  
- **OpenStack:** Understand each component, storage types, and VM workflow  
- **Flashcards:** Make cards for metrics, roles, and workflows  
- **GitHub Tip:** Upload to `NPTEL_Cloud_Computing/Week3/week3_cheatsheet.md`  
- **Study Tip:** Review 15 mins daily with `week3_explanation.md`

