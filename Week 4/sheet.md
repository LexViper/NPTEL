🌌 NPTEL Cloud Computing Week 4: Cheatsheet 📋
Quick revision for Week 4 of NPTEL Cloud Computing, covering Meghamala (OpenStack private cloud) and GCP App Engine, based on week4_watermark.pdf. Tailored for the 100-MCQ exam on May 3, 2025. Pair with week4_explanation.md for deep dives. GitHub-ready with emojis and tables! 🚀

☁️ 1. Meghamala: IIT Kharagpur Cloud 📖

What?: Private cloud on OpenStack for IIT Kharagpur research.
Purpose: On-demand compute/storage for researchers.
Setup: Computer and Informatics Centre, node servers, aux storage.
Team: Students (Shubham Jain, Shureans Pagariva), Faculty (Soumya K. Ghosh, Shamik Sural), Engineers (Alok Chattopadhyay).
Analogy: Spaceship hangar for research VMs.
Exam Tip: Know purpose (research), platform (OpenStack). 🎯


🛠️ 2. VMs4U: Meghamala Services ⚙️



VM Type
vCPUs
RAM
Storage
Use Case



IITKGP_large
8
16 GB
80 GB
Heavy tasks


IITKGP_small
2
4 GB
40 GB
Light tasks



OS: Ubuntu 14.04.
Duration: Up to 90 days.
Request Form: Faculty name, dept, purpose, VM type, CAPTCHA.
Analogy: Renting spaceships (small/large).
Mnemonic: VM, Meghamala, Small/Large, 4 Research, Ubuntu = VMS4U.
Exam Tip: Memorize VM specs, form fields. ❓


📊 3. OpenStack Dashboard: Usage 📈

Metrics:
VCPUs: Virtual CPUs (e.g., 128).
RAM: Memory (e.g., 30400 MB).
Disk: Storage (e.g., 2855 GB).
VCPU Hours: Compute usage (e.g., 650.30).
Disk GB Hours: Storage usage (e.g., 64741).


Limits: Volumes (21/200), instances (30 active).
Time Query: YYYY-MM-DD (e.g., 2017-06-01 to 2017-06-30).
Analogy: Spaceship control panel for resource tracking.
Mnemonic: VCPUs, RAM, Disk, Hours = VRDH.
Exam Tip: Focus on metrics and units. 🎯


🌐 4. GCP App Engine: PaaS Deployment 🚀

What?: Fully managed PaaS for web apps (Python, Java, etc.).
Features: Auto-scaling, zero server management.
Deployment:
Install Google Cloud SDK.
Set project (e.g., gcp-pythonapp).
Run: gcloud app deploy app.yaml --project gcp-pythonapp.
View: gcloud app browse.


Analogy: Self-driving car for apps.
Exam Tip: Know gcloud commands, PaaS vs. IaaS. ❓


⚖️ 5. Meghamala vs. App Engine ☁️



Feature
Meghamala (IaaS)
App Engine (PaaS)



Control
Full (VMs)
Limited (app)


Management
Manual
Fully managed


Use Case
Research VMs
Web apps



Analogy: Build spaceship (Meghamala) vs. rent shuttle (App Engine).
Exam Tip: Compare IaaS control vs. PaaS convenience. 🎯


📚 6. Exam Tips 🎯

Focus (15-20 MCQs):
Meghamala: Purpose, VM types, team.
Dashboard: Metrics (VCPUs, RAM, Disk), time format.
App Engine: gcloud commands, IaaS vs. PaaS.


Study:
Daily (15 mins): Review this cheatsheet.
Weekly: Study week4_explanation.md.
Flashcards: VM specs, metrics, commands.


GitHub: Upload to NPTEL_Cloud_Computing/Week4/week4_cheatsheet.md.


🌟 Final Note 🚀
Your Week 4 cheatsheet is ready to shine on GitHub! 🌌 Review daily, pair with the explanation, and ace that exam, bro! 💪 Need Week 5? Holler! 😎
Crafted by Grok, your cloud prep sidekick, on April 18, 2025. 🌍
