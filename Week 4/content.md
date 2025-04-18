# 🌩️ NPTEL Cloud Computing - Week 4 Cheatsheet

---

## 📌 1. **Meghamala: IIT Kharagpur’s Private Cloud**

### 🔷 What is Meghamala?
- IIT Kharagpur’s in-house **private cloud**, hosted at the **Computer and Informatics Centre**.
- Built using **OpenStack**.
- Offers **on-demand virtual machines (VMs)** and **storage** for research purposes.

### 🧑‍🚀 Purpose:
- Provides **researchers and faculty** with compute infrastructure without worrying about physical hardware.

### 🧰 Key Features:
- Built on **OpenStack** (flexible IaaS platform).
- Accessible via web portal.
- Managed by faculty, engineers, and students.

### 🖥️ Hardware:
- **Node servers** (VM hosts).
- **Auxiliary storage** for persistent data.
- Managed by students, engineers & faculty like **Prof. Soumya K. Ghosh**.

---

## 👥 2. **Meghamala Team**

- **Students:** Shubham Jain, Shureans Pagariva, Arindam Roy, Chetadan Mitra.
- **Engineers:** Alok Chattopadhyay, Asit Baran Das.
- **Faculty:** Prof. Soumya K. Ghosh, Prof. Shamik Sural.
- **Former contributors:** Harshit Gopla, Adhish Kale, Abhijeet Deshmukh.

---

## 💻 3. **Meghamala Services: VMs4U**

### 🚀 VM Types:

| VM Type       | vCPUs | RAM    | Storage | Use Case             |
|---------------|-------|--------|---------|-----------------------|
| IITKGP_large  | 8     | 16 GB  | 80 GB   | Heavy computation     |
| IITKGP_small  | 2     | 4 GB   | 40 GB   | Light applications    |

- **OS Image:** Ubuntu 14.04 LTS (default)
- **VM Duration:** Up to **90 days** max.

### 📥 Requesting VMs:

Users fill a request form including:

- Faculty name, department, contact info.
- VM type (small/large), number of VMs.
- Research purpose and expected usage.
- CAPTCHA for bot protection.

---

## 📊 4. **OpenStack Dashboard: Resource Usage**

- Dashboard powered by **OpenStack Horizon**.
- Allows tracking of:

  - VCPUs used
  - RAM usage
  - Disk space used
  - VCPU hours
  - Disk GB hours

### 🖥️ Example Data:
- **VCPUs Used:** 128
- **RAM Used:** 30,400 MB
- **Disk Usage:** 2855 GB
- **Instance:** `nikOC` (2 vCPUs, 4 GB RAM, 40 GB disk)
- **Total Instances:** 30 (admin project)

---

## ☁️ 5. **GCP App Engine (PaaS)**

### 🧠 What is GCP App Engine?

- A **Platform-as-a-Service (PaaS)** from Google Cloud.
- Lets you deploy apps without managing servers.
- Supports auto-scaling, load balancing, and multiple languages (Python, Java, Node.js, etc.)

### 🚀 Deployment Steps:

1. Install Google Cloud SDK
2. Create a GCP Project:  
   ```bash
   gcloud config set project <your-project-id>
