

# 🌌 NPTEL Cloud Computing Week 4: Cheatsheet 📋

---

## ☁️ 1. Meghamala: IIT Kharagpur Cloud 📖

- **What?**: Private cloud on **OpenStack** for IIT Kharagpur research.
- **Purpose**: On-demand compute/storage for researchers.
- **Setup**: Computer and Informatics Centre, node servers, auxiliary storage.
- **Team**:
  - **Students**: Shubham Jain, Shureans Pagariva
  - **Faculty**: Soumya K. Ghosh, Shamik Sural
  - **Engineers**: Alok Chattopadhyay
- **Analogy**: Spaceship hangar for research VMs.
- **Exam Tip**: Know purpose (research), platform (OpenStack). 🎯

---

## 🛠️ 2. VMs4U: Meghamala Services ⚙️

### 💻 VM Types

| VM Type        | vCPUs | RAM    | Storage | Use Case       |
|----------------|-------|--------|---------|----------------|
| IITKGP_large   | 8     | 16 GB  | 80 GB   | Heavy tasks    |
| IITKGP_small   | 2     | 4 GB   | 40 GB   | Light tasks    |

- **OS**: Ubuntu 14.04  
- **Duration**: Up to **90 days**  
- **Request Form Includes**:
  - Faculty name
  - Department
  - Purpose
  - VM type
  - CAPTCHA

- **Analogy**: Renting spaceships (small/large).  
- **Mnemonic**: VM, Meghamala, Small/Large, 4 Research, Ubuntu = **VMS4U**  
- **Exam Tip**: Memorize VM specs, form fields. ❓

---

## 📊 3. OpenStack Dashboard: Usage 📈

### 📏 Metrics:

- **VCPUs**: Virtual CPUs (e.g., 128)
- **RAM**: Memory (e.g., 30,400 MB)
- **Disk**: Storage (e.g., 2,855 GB)
- **VCPU Hours**: Compute usage (e.g., 650.30)
- **Disk GB Hours**: Storage usage (e.g., 64,741)

- **Limits**:
  - Volumes: 21/200
  - Instances: 30 active

- **Time Query Format**: `YYYY-MM-DD` (e.g., 2017-06-01 to 2017-06-30)
- **Analogy**: Spaceship control panel for resource tracking  
- **Mnemonic**: VCPUs, RAM, Disk, Hours = **VRDH**  
- **Exam Tip**: Focus on metrics and units. 🎯

---

## 🌐 4. GCP App Engine: PaaS Deployment 🚀

- **What?**: Fully managed **PaaS** for web apps (Python, Java, etc.)
- **Features**: Auto-scaling, zero server management

### 🚀 Deployment Steps:

1. **Install** Google Cloud SDK
2. **Set project**:  
   ```bash
   gcloud config set project <your-project-id>

	3.	Deploy app:

gcloud app deploy app.yaml --project <your-project-id>


	4.	View app:

gcloud app browse



	•	Analogy: Self-driving car for apps
	•	Exam Tip: Know gcloud commands, PaaS vs. IaaS. ❓

⸻

⚖️ 5. Meghamala vs. App Engine ☁️

Feature	Meghamala (IaaS)	App Engine (PaaS)
Control	Full (VMs)	Limited (app only)
Management	Manual	Fully managed
Use Case	Research VMs	Web apps

	•	Analogy: Build spaceship (Meghamala) vs. rent shuttle (App Engine)
	•	Exam Tip: Compare IaaS control vs. PaaS convenience. 🎯

⸻

📚 6. Exam Tips 🎯

🔍 Focus (15–20 MCQs likely):
	•	Meghamala: Purpose, VM types, team
	•	Dashboard: Metrics (VCPUs, RAM, Disk), time format
	•	App Engine: gcloud commands, IaaS vs. PaaS

📖 Study Plan:
	•	Daily (15 mins): Review this cheatsheet
	•	Weekly: Study week4_explanation.md
	•	Flashcards: VM specs, metrics, GCP commands

⸻

📁 GitHub Tip

📂 Path: NPTEL_Cloud_Computing/Week4/week4_cheatsheet.md

⸻
