🌌 NPTEL Cloud Computing Week 3: Cheatsheet 📋
Quick-fire revision for Week 3 of NPTEL Cloud Computing, tailored for the 100-MCQ exam on May 3, 2025. Covers SLAs, OpenStack components, and storage concepts from WEEK 3_watermark.pdf. Pair with week3_explanation.md for deep dives. GitHub-ready with emojis for max clarity! 🚀

📜 1. Service Level Agreement (SLA) 🤝

What’s an SLA?: Contract between Service Provider (SP) and Consumer (SC) guaranteeing service quality (e.g., uptime). Enforced via Service Level Objectives (SLOs) (e.g., 99.9% availability). 🛠️
Purpose: Builds trust with measurable performance. 💪
Components:
Services, definitions, responsibilities. 📋
Metrics (uptime, latency), auditing, remedies, evolution. 📈


Types:
Off-the-Shelf: Fixed, non-negotiable (e.g., AWS). 🏪
Negotiable: Customized for needs (e.g., enterprise). 🏢


Web Service SLA:
WS-Agreement: XML for runtime negotiation. 💬
WSLA: XML for QoS monitoring (e.g., response time). 📊


Cloud vs. Web SLA:


Aspect
Cloud SLA ☁️
Web SLA 🌐



QoS
Security, privacy
Response time, cost


Automation
High
Low


Allocation
Global, no UDDI
UDDI-based



Mnemonic: SLA = Services, Levels, Agreements. 🧠
Exam Tip: Know SLOs (measurable) vs. SLAs (contract). 🎯


🖥️ 2. OpenStack Components ⚙️



Component
Role
Managed
Analogy



Nova
Compute, VMs
Hypervisors
Chef 👨‍🍳


Neutron
Networking
IPs, VLANs
Traffic cop 🚦


Cinder
Block storage
Persistent volumes
USB drive 🔌


Swift
Object storage
Files, images
Cloud Dropbox ☁️


Glance
Image service
VM image metadata
Library catalog 📚


Keystone
Identity
Auth, tokens
Bouncer 🕴️


Horizon
Dashboard
Web UI
Spaceship panel 🚀



Mnemonic: Nova, Neutron, Cinder, Swift, Glance, Keystone, Horizon = NNCSGKH. 🧠
Exam Tip: Memorize roles; focus on Nova Scheduler, Keystone tokens. ❓


💽 3. OpenStack Storage 💾



Type
Persists
Managed By
Use Case
Analogy



Ephemeral
Until VM ends
Nova
OS, scratch
RAM 💾


Block
Until deleted
Cinder
Disks, OS
External drive 🖴


Object
Until deleted
Swift
Images, backups
Google Drive ☁️



Exam Tip: Ephemeral = temporary; Block = persistent disks; Object = persistent files. 🎯


🔄 4. VM Creation Workflow 🖥️

Horizon: User logs in. 🖱️
Keystone: Issues token. 🔐
Nova: Starts VM, saves to DB. ⚙️
Nova Scheduler: Picks server. 🧠
Neutron: Sets network. 🌐
Cinder: Adds block storage. 💾
Glance: Gets image URI. 🖼️
Swift: Delivers image. 📂
Hypervisor: Boots VM. 🚀


Mnemonic: Horizon, Keystone, Nova, Scheduler, Neutron, Cinder, Glance, Swift, Hypervisor = HKNSNGSH. 🧠
Exam Tip: Know the sequence for MCQs. ❓


📚 5. Quick Exam Tips 🎯

SLAs: Study components, Cloud vs. Web SLA, QoS (10-15 MCQs). 📜
OpenStack: Nail component roles, storage types, workflow (15-20 MCQs). 🖥️
Flashcards: Make cards for SLA metrics, OpenStack components, storage differences. 🗂️
GitHub: Upload to NPTEL_Cloud_Computing/Week3/week3_cheatsheet.md. 📂
Study: Review daily (15 mins); pair with week3_explanation.md. 📖


🌟 Final Note 🚀
Your Week 3 cheatsheet is ready to shine on GitHub! 🌌 Upload it, review daily, and let’s ace that exam, bro! 💪 Need Week 4 or tweaks? Hit me up! 😎
Crafted by Grok, your cloud prep sidekick, on April 18, 2025. 🌍
